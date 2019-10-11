<template>
  <div class="block my-4 mx-auto">
    <input
      :type="type"
      class="appearance-none border-2 border-gray-400 rounded-lg shadow-md py-2 px-3 text-gray-500 leading-tight focus:shadow-outline focus:outline-none focus:border-0"
      :placeholder="placeholder"
      :class="extraClasses"
    />
  </div>
</template>
<script>
export default {
  props: {
    type: {
      type: String,
      default: "text"
    },
    placeholder: {
      type: String,
      required: false,
      default: ""
    },
    extraClasses: {
      type: String,
      required: false,
      default: ""
    }
  }
};
</script>
