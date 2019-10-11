<template>
  <div class="my-4 mx-auto">
    <button
      class="text-white font-bold px-5 py-2 rounded shadow-md"
      :class="[color, hoverComputed, extraClasses]"
    >
      {{ this.value }}
    </button>
  </div>
</template>
<script>
export default {
  computed: {
    hoverComputed() {
      if (this.hoverColor) {
        return `hover:${this.hoverColor}`;
      }
      if (this.color) {
        let colorSplit = this.color.split("-");
        colorSplit[colorSplit.length - 1] = 700;
        return `hover:${colorSplit.join("-")}`;
      }
      return "hover:bg-blue-700";
    }
  },
  props: {
    color: {
      type: String,
      default: "bg-blue-400"
    },
    hoverColor: {
      type: String
    },
    extraClasses: {
      type: String,
      required: false,
      default: ""
    },
    value: {
      type: String,
      required: true
    }
  }
};
</script>
<style lang="scss"></style>
