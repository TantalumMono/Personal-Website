<template>
  <div class="fixed top-0 left-0 w-full flex justify-center mt-4 z-50">
    <div class=" inline-flex bg-base-100 backdrop-filter backdrop-blur-lg bg-opacity-50 rounded-lg shadow-lg px-4 py-2">
      <div class="flex-1">
        <a class="btn btn-ghost text-xl" href="#home">Home</a>
      </div>

      <div class="flex-1">
        <a class="btn btn-ghost text-xl" href="#work">Work</a>
      </div>
      <div class="flex-1">
        <a class="btn btn-ghost text-xl" href="#gallery">Gallery</a>
      </div>
      <div class="flex-1">
        <a class="btn btn-ghost text-xl" href="#other">Other</a>
      </div>
      <div class="flex-1">
        <a class="btn btn-ghost text-xl" href="./assets/resume.pdf">Resume</a>
      </div>
      <!-- 主题切换 -->
      <label class="swap swap-rotate">
        <!-- this hidden checkbox controls the state -->
        <input type="checkbox" class="theme-controller" @change="toggleTheme" />

        <!-- sun icon -->
        <svg class="swap-off fill-current w-10 h-10" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M5.64,17l-.71.71a1,1,0,0,0,0,1.41,1,1,0,0,0,1.41,0l.71-.71A1,1,0,0,0,5.64,17ZM5,12a1,1,0,0,0-1-1H3a1,1,0,0,0,0,2H4A1,1,0,0,0,5,12Zm7-7a1,1,0,0,0,1-1V3a1,1,0,0,0-2,0V4A1,1,0,0,0,12,5ZM5.64,7.05a1,1,0,0,0,.7.29,1,1,0,0,0,.71-.29,1,1,0,0,0,0-1.41l-.71-.71A1,1,0,0,0,4.93,6.34Zm12,.29a1,1,0,0,0,.7-.29l.71-.71a1,1,0,1,0-1.41-1.41L17,5.64a1,1,0,0,0,0,1.41A1,1,0,0,0,17.66,7.34ZM21,11H20a1,1,0,0,0,0,2h1a1,1,0,0,0,0-2Zm-9,8a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V20A1,1,0,0,0,12,19ZM18.36,17A1,1,0,0,0,17,18.36l.71.71a1,1,0,0,0,1.41,0,1,1,0,0,0,0-1.41ZM12,6.5A5.5,5.5,0,1,0,17.5,12,5.51,5.51,0,0,0,12,6.5Zm0,9A3.5,3.5,0,1,1,15.5,12,3.5,3.5,0,0,1,12,15.5Z" />
        </svg>

        <!-- moon icon -->
        <svg class="swap-on fill-current w-10 h-10" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M21.64,13a1,1,0,0,0-1.05-.14,8.05,8.05,0,0,1-3.37.73A8.15,8.15,0,0,1,9.08,5.49a8.59,8.59,0,0,1,.25-2A1,1,0,0,0,8,2.36,10.14,10.14,0,1,0,22,14.05,1,1,0,0,0,21.64,13Zm-9.5,6.69A8.14,8.14,0,0,1,7.08,5.22v.27A10.15,10.15,0,0,0,17.22,15.63a9.79,9.79,0,0,0,2.1-.22A8.11,8.11,0,0,1,12.14,19.73Z" />
        </svg>
      </label>
    </div>
  </div>
  <div id="home" class="block h-16"></div>
  <div class="container mx-auto p-4 bg-base-100 shadow-xl rounded-lg my-8  max-w-4xl">

    <article class="prose max-w-none">
      <h1 class="hover-grow-hover">🙌<span class="text-gray-300 ">Hi there!</span> I'm 马砚文(Yanwen Ma) </h1>
      <p>I am a fourth-year undergraduate student at the School of Sports Engineering (SSE), Beijing Sport University, expected to graduate in 2025. Recently, I have received a master's offer from <b>BUAA</b>, base in HangZhou, where I will pursue my graduate studies in Computer Science, with a research focus on 3D Computer Vision.</p>
      <p>I'm currently seeking an internship opportunity related to 3D Computer Vision, computer graphics, or related fields. </p>
      <!-- <span class="font-bold">PLZ</span> check out my <a
          href="/src/assets/resume.pdf" class="link link-primary ">Resume</a> here. -->
      <h2>Interests</h2>
      <p class="flex flex-wrap px-4 gap-x-2 gap-y-2 items-end">
        <button class="btn btn-sm btn-error mb-2">Multy-LLM</button>
        <button class="btn btn-xs btn-warning mb-2">Game Dev</button>
        <button class="btn btn-sm btn-info mb-2">Agents in Games</button>

        <button class="btn btn-xs btn-success mb-2">3D AIGC</button>
        <button class="btn btn-xs btn-warning mb-2">Computer graphics</button>
      </p>

    </article>

  </div>
  <div class="container mx-auto p-4 bg-base-100 shadow-xl rounded-lg my-8 max-w-4xl">

    <div id="work">
      <!-- detail -->
      <article class="prose max-w-full  break-words">
        <h1>Work</h1>
        <div class="card lg:card-side card-compact bg-base-100 shadow-xl">
          <figure><img src="./assets/avatarsoul.png" alt="AvatarSoul" /></figure>
          <div class="card-body">
            <h2 class="card-title">AvatarSoul</h2>
            <p>Fully LLM-driven avatars</p>
            <p>📣This work has advanced to the finals of 4CBJ2024.🎉</p>
            <div class="card-actions justify-end">
              <a href="https://github.com/Gelercatty/AvatarSoul" target="_blank">
                <button class="btn btn-primary">Code</button>
              </a>
              <a href="https://www.bilibili.com/video/BV1gr42177QF" target="_blank">
                <button class="btn btn-primary">Video Demo</button>
              </a>
            </div>
          </div>
        </div>

        <div class="card lg:card-side card-compact bg-base-100 shadow-xl">
          <figure><img src="./assets/taichi.png" alt="AvatarSoul" /></figure>
          <div class="card-body">
            <h2 class="card-title">TaiChiGPT</h2>
            <p>Complex Sports Action Generation Based on Large Language Models</p>
            <p> Jianwei Li<sup>1</sup>, Kehao Ran<sup>1</sup>, <strong>Yanwen Ma<sup>1</sup></strong>, Hongwen
              Xie<sup>2</sup>.</p>
            <p>👨‍🔬👩‍🔬This work has been submitted to the IEEE 2025.</p>
            <div class="card-actions justify-end">
              <a href="https://bsu3dvlab.github.io/TaiChi24/index.html">
                <button class="btn btn-primary">Dataset</button>
              </a>
              <a href="https://youtu.be/u2j5-0emYc8?si=z5eQruwtmQyQmW9i" target="_blank" class="tooltip  tooltip-accent" data-tip="may need Vpn">
                <button class="btn btn-primary ">Video Demo</button>

              </a>
            </div>
          </div>
        </div>
        <div class="card lg:card-side card-compact bg-base-100 shadow-xl">
          <figure><img src="./assets/eyesnow.png" alt="AvatarSoul" /></figure>
          <div class="card-body">
            <h2 class="card-title">EyeSnow</h2>
            <p>A snowfield tracking and shooting system based on YOLO and gimbal control algorithms.</p>

            <ul class="list-none pl-0">
              <li>💪Beijing Sport University Innovation Training Project, funding of 3k.</li>
              <li>🏆4CBJ2023 National Third Prize</li>
              <li>🏆202e China College Students’ 'Internet+' Innovation and Entrepreneurship Competition, Beijing
                Competition Area Third Prize</li>
              <li>🎉Finalist in the China Sports Equipment Intelligent Manufacturing Competition</li>
            </ul>
            <div class="card-actions justify-end">
              <a href="https://github.com/Gelercatty/SnowEye" target="_blank">
              <button class="btn btn-primary">Code</button>
              </a>
            </div>
          </div>
        </div>
      </article>
    </div>
  </div>


  <div class="container mx-auto p-4 bg-base-100 shadow-xl rounded-lg my-8 max-w-4xl">

    <div id="other" class="prose max-w-none">

      <div>
        <h1>🥇Selected Honors</h1>

        <article class="prose max-w-none">
          <div class="flex justify-between items-center py-1 hover-grow-hover">
            <span>CUMCU Beijing area First Prize</span>
            <span class="flex-grow border-t border-dotted border-gray-400 mx-2"></span>
            <span>2023</span>
          </div>
          <div class="flex justify-between items-center py-1 hover-grow-hover">
            <span>Computer Design Competition National Third Prize</span>
            <span class="flex-grow border-t border-dotted border-gray-400 mx-2"></span>
            <span>2023</span>
          </div>
          <div class="flex justify-between items-center py-1 hover-grow-hover">
            <span>Undergraduate First-Class Scholarship</span>
            <span class="flex-grow border-t border-dotted border-gray-400 mx-2"></span>
            <span>2023</span>
          </div>
          <div class="flex justify-between items-center py-1 hover-grow-hover">
            <span>Beijing Sport University Outstanding Student</span>
            <span class="flex-grow border-t border-dotted border-gray-400 mx-2"></span>
            <span>2024</span>
          </div>
          <div class="flex justify-between items-center py-1 hover-grow-hover">
            <span>优秀共青团员</span>
            <span class="flex-grow border-t border-dotted border-gray-400 mx-2"></span>
            <span>2024</span>
          </div>

          <p></p>

          <h1>🎓Experience</h1>
          <div class="flex justify-between items-center py-1 hover-grow-hover">
            <span>Publicity Minister of SSE Student Union</span>
            <span class="flex-grow border-t border-dotted border-gray-400 mx-2"></span>
            <span>2022.3 - 2023.6</span>
          </div>
          <div class="flex justify-between items-center py-1 hover-grow-hover">
            <span>President of BSU Guitar Club</span>
            <span class="flex-grow border-t border-dotted border-gray-400 mx-2 "></span>
            <span>2022.9 - present</span>
          </div>
        </article>
      </div>
    </div>
  </div>

  <div class="container mx-auto p-4 bg-base-100 shadow-xl rounded-lg my-8 max-w-4xl">
    <div id="gallery" class="prose max-w-none">
      <h1>Gallery</h1>

      <div tabindex="0" class="collapse collapse-arrow border border-base-300 bg-base-200">
        <input type="checkbox" />
        <div class="collapse-title text-xl font-medium">
          My art works, my band, and my CAT... 😼
        </div>
        <div class="collapse-content">


          <div class="columns-1 sm:columns-2 lg:columns-3 gap-4">
            <div class="mb-4 break-inside-avoid-column">
              <img @click='openModal("./assets/gallery/1.png")' src="./assets/gallery/1.png" alt="Gallery Image 1"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/2.png')" src="./assets/gallery/2.png" alt="Gallery Image 2"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/3.png')" src="./assets/gallery/3.png" alt="Gallery Image 3"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/4.png')" src="./assets/gallery/4.png" alt="Gallery Image 4"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/5.png')" src="./assets/gallery/5.png" alt="Gallery Image 5"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/6.png')" src="./assets/gallery/6.png" alt="Gallery Image 6"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/7.png')" src="./assets/gallery/7.png" alt="Gallery Image 7"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/8.png')" src="./assets/gallery/8.png" alt="Gallery Image 8"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/9.png')" src="./assets/gallery/9.png" alt="Gallery Image 9"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <!-- <div class="mb-4 break-inside-avoid-column">
          <img @click="openModal('/assets/gallery/10.png')" src="./assets/gallery/10.png" alt="Gallery Image 10"
            class="w-full h-auto rounded-lg shadow-md cursor-pointer">
        </div> -->
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/11.png')" src="./assets/gallery/11.png" alt="Gallery Image 11"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>
            <div class="mb-4 break-inside-avoid-column">
              <img @click="openModal('./assets/gallery/12.png')" src="./assets/gallery/12.png" alt="Gallery Image 12"
                class="w-full h-auto rounded-lg shadow-md cursor-pointer">
            </div>

            <!-- 添加更多图片 -->
          </div>



        </div>
      </div>





    </div>
  </div>




  <footer class="footer footer-center p-10 bg-primary text-primary-content">
    <aside>


      <div class="avatar">
        <div class="w-24 rounded-full">
          <img src="/src/assets/avatar.png" />
        </div>
      </div>

      <p class="font-bold">
        GelerCAT =w= <br>Code, Love, and Create
      </p>
      <p>Email : Gelercat@bsu.edu.cn</p>
      <p>H: 130 2762 7852 </p>
    </aside>

  </footer>




  <!-- Modal -->
  <div v-if="modalVisible" class="modal modal-open flex justify-center items-center">
    <div class="modal-box relative max-w-3xl">
      <button @click="closeModal" class="btn btn-sm btn-circle absolute right-2 top-2">✕</button>
      <img :src="modalImage" :alt="modalImage" class="w-full h-auto rounded-lg shadow-md">
    </div>
  </div>

</template>


<script>
import { ref, watch, onMounted } from 'vue';
export default {
  setup() {
    const theme = ref('light');  // 默认主题为 'light'
    const modalVisible = ref(false);
    const modalImage = ref("");

    function toggleTheme(event) {
      theme.value = event.target.checked ? 'dark' : 'light';
    }

    function openModal(image) {
      modalImage.value = image;
      modalVisible.value = true;
    }
    function closeModal() {
      modalVisible.value = false;
      modalImage.value = '';
    }







    watch(theme, (newTheme) => {
      document.documentElement.setAttribute('data-theme', newTheme);
    });

    onMounted(() => {
      document.documentElement.setAttribute('data-theme', theme.value);
    });






    return {
      toggleTheme,
      modalVisible,
      modalImage,
      openModal,
      closeModal,
    };
  }
}
</script>


<style>
/* 确保图片容器在列内不被断开 */
.break-inside-avoid-column {
  break-inside: avoid;
}

/* DaisyUI Modal Styles */
.modal.modal-open {
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal-box {
  max-width: 90%;
  max-height: 90%;
  overflow: auto;
}


/* 自定义悬停动画 */
.hover-grow-hover {
  transition: transform 0.15s ease-in-out;
}

.hover-grow-hover:hover {
  transform: scale(1.005) translateY(-5px);
}
</style>
