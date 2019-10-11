<template>
  <div class="w-full max-w-sm mt-4">
    <form action="#" class="bg-gray-200 shadow-md rounded p-5">
      <div class="mb-4">
        <label for="input--username" class="text-black font-bold font-base"
          >Username</label
        >
        <Input
          type="text"
          id="input--username"
          placeholder="Enter Username"
          extraClasses="w-full rounded"
        />
      </div>
      <div class="mb-5">
        <label for="input--password" class="text-black font-bold font-base"
          >Password</label
        >
        <Input
          type="text"
          id="input--password"
          placeholder="***********"
          extraClasses="border-2 border-red-500 w-full rounded"
        />
      </div>
      <p class="text-xs text-red-400 italic mb-5">Please choose a password.</p>
      <div class="flex flex-wrap justify-between items-center">
        <Button
          extraClasses="py-2 px-6 focus:outline-none focus:shadow-outline shadow-none"
          value="Sign In"
        />
        <a
          href="#"
          class="inline-block text-blue-500 font-bold text-sm hover:text-blue-800 align-baseline"
          >Forgot Password?</a
        >
      </div>
    </form>
  </div>
</template>

<script>
import Input from "./input.vue";
import Button from "./button.vue";
export default {
  name: "LoginForm",
  components: {
    Input,
    Button
  }
};
</script>

<style lang="css" scoped></style>
