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
    
  </footer>
</template>

<style>
.phone-body {
  @apply w-[360px] h-screen border border-solid border-[#9f2ae8] border-t-4 p-2;
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
</style>
