<script setup></script>

<template>
  <section class="bg-indigo-950 p-16 flex items-center justify-between">
    <div class="basis-1/2">
      <h1 class="text-5xl font-semibold mb-8">Contact Me</h1>
    </div>
    <form ref="form" @submit.prevent="sendEmail" class="grow">
      <div class="mb-5">
        <label class="flex flex-col-reverse">
          <input
            type="text"
            name="user_name"
            class="min-w-full bg-transparent border-b border-pink-500 peer"
          />
          <span
            class="inline-block transition translate-y-2/4 peer-focus:translate-y-0"
            >Name</span
          >
        </label>
      </div>
      <div class="mb-5">
        <label class="flex flex-col-reverse">
          <input
            type="email"
            name="user_email"
            class="min-w-full bg-transparent border-b border-pink-500 peer"
          />
          <span
            class="inline-block transition translate-y-2/4 peer-focus:translate-y-0"
            >Email</span
          >
        </label>
      </div>
      <div class="mb-5">
        <label class="flex flex-col-reverse">
          <textarea
            name="message"
            class="resize-none min-w-full bg-transparent border-b border-pink-500 peer"
          ></textarea>
          <span
            class="inline-block transition translate-y-full peer-focus:translate-y-0"
            >Message</span
          >
        </label>
      </div>
      <input
        type="submit"
        value="Send"
        class="cursor-pointer border-b-2 border-pink-500"
      />
    </form>
  </section>
</template>
