<template>
  <main>
    <div class="phone-body">
      <div class="chat-view">
        <img
          class="img-icon"
          src="@/assets/user-profile-icon-left.svg"
          alt="profile icon"
        />
        <div class="chat-box bg-[#9f2ae8] triangle left-top">
          <div class="chat-text">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
          </div>
        </div>
      </div>
      <div class="chat-view">
        <div class="chat-box bg-[#d3d3d3] triangle right-top">
          <div class="chat-text">
            <p>Lorem ipsum dolor sit amet, consectetur</p>
          </div>
        </div>
        <img
          class="img-icon"
          src="@/assets/user-profile-icon-right.svg"
          alt="profile icon"
        />
      </div>
      <div class="chat-view">
        <div class="chat-box bg-[#d3d3d3] triangle right-top">
          <div class="chat-text">
            <p>Lorem ipsum dolor</p>
          </div>
        </div>
        <img
          class="img-icon"
          src="@/assets/user-profile-icon-right.svg"
          alt="profile icon"
        />
      </div>
      <div class="chat-view">
        <img
          class="img-icon"
          src="@/assets/user-profile-icon-left.svg"
          alt="profile icon"
        />
        <div class="chat-box bg-[#9f2ae8] triangle left-top">
          <div class="chat-text">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing</p>
          </div>
        </div>
      </div>
    </div>
  </main>
  <footer>
    <div class="content form-height">
      <form>
        <input
          name="thought"
          type="text"
          class="form-input"
          placeholder="Start typing"
        />
        <button type="submit" class="form-button">Send</button>
      </form>
    </div>
  </footer>
</template>

<style>
.phone-body {
  @apply w-[360px] h-auto border border-solid border-[#9f2ae8] border-t-4 p-2;
}

.img-icon {
  @apply w-12 pb-10;
}

.chat-view {
  @apply flex justify-center;
}

.chat-box {
  @apply h-auto w-[200px] relative inline-block m-5;
}

.triangle.left-top:after {
  @apply w-0 h-0 top-0 right-auto -left-5 bottom-auto absolute content-[""];
  border: 22px solid;
  border-color: #9f2ae8 transparent transparent transparent;
}

.triangle.right-top:before {
  border: 32px solid;
  @apply w-0 h-0 top-0 -right-5 left-auto bottom-auto absolute content-[""];
  border-color: #d3d3d3 transparent transparent transparent;
}

.chat-text {
  @apply p-3;
}

.chat-text p {
  @apply text-white text-xs;
}

footer {
  @apply bg-[#9f2ae8] p-1;
}

form {
  @apply flex;
}
.form-height {
  @apply h-32;
}

.content {
  @apply text-[#262626] py-2 w-full h-auto px-2 mb-1;
}

.form-input {
  @apply rounded-xl w-full h-[2.5rem] px-6 focus:outline-none text-sm bg-gray-100 text-[#AAAAAA] appearance-none
   py-2 focus:border placeholder-gray-500 focus:bg-[white] focus:ring-[#B8CADE] focus:border-[#B8CADE] focus:z-10;
}

.form-button {
  @apply h-[2.5rem] w-4/12 ml-4 py-2 px-4 border border-transparent !bg-gray-100 text-sm font-medium rounded-xl text-black cursor-pointer;
}
</style>
