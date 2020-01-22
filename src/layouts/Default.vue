<template>
  <div class="font-sans sm:mx-2 sm:p-2 lg:mx-auto container">


    <header class="h-30">
      <strong>
        <g-link class="visible text-5xl text-gray-600" to="/">{{ $static.metaData.siteName }}</g-link>
      </strong>
      <nav class="nav text-lg">
        <g-link class="mx-2 text-gray hover:text-gray-500" to="/">Home</g-link>
        <g-link class="mx-2 text-gray hover:text-gray-500" to="/about">About</g-link>
      </nav>
    </header>

    <slot/>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>
