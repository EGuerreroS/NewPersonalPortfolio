<script setup>
import { ref, onMounted } from 'vue'

const video = ref(null)

onMounted(() => {
  const observer = new IntersectionObserver(
    (entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          video.value.play()
        } else {
          video.value.pause()
        }
      })
    },
    { threshold: 0.1 } // cuando el 50% del video sea visible
  )

  observer.observe(video.value)
})
</script>

<template>
  <div class=" q-mx-xl q-px-xl q-my-xl">
    <div class="row inline q-gutter-sm">
      <div class=""><h4 class="txSolid">SOME</h4></div>
      <div class=""><h4 class="secondTxOutlined">PROJECTS</h4></div>
    </div>
    <div>
      <!-- PROYECTO -->
      <div class="row q-mx-md q-mb-xl q-pr-xl">
        <div class="col-4">
          <!-- PROJECT NAME -->
          <div class="row inline q-gutter-sm">
            <div class=""><h5 class="txSolid q-mt-none q-mb-md">SMART</h5></div>
            <div class=""><h5 class="secondTxOutlined q-mt-none q-mb-md">ACCESS</h5></div>
          </div>
          <div class="row q-mt-sm  project-card">
            <div class="column  col justify-around q-mb-md q-ml-md">
              <div class="col ">
                <q-icon
                  name="arrow_drop_down"
                  color="purple-14"
                  size="lg"
                />
                </div>
              <div class="col">
                <q-icon
                  name="keyboard_double_arrow_right"
                  color="purple-14"
                  size="lg"
                />
              </div>
              <div class="col just">
                <h6 class="text-purple-14 q-my-none">SMART ACCESS</h6>
              </div>

            </div>
            <div class="col justify-end text-right text-yellow text-h6 content-end q-mr-md q-mb-md">01</div>
          </div>
          <!-- DESCRIPTION  -->
          <div class="text-justify text-white q-mt-md">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolor eaque id iure nostrum odit possimus
              quisquam quos voluptate? Dolor ex mollitia, nam numquam praesentium quaerat reiciendis rem similique! A
              accusamus, animi aperiam at cumque delectus distinctio dolorem est eum eveniet fuga id, ipsum, itaque
              laboriosam maiores obcaecati placeat quia veritatis</p>
          </div>
          <!-- EXTRA DATA -->
          <div class="">
            <div class="row items-center q-mb-lg ">
              <div class="q-mr-sm">
                <q-icon
                  color="yellow"
                  name="alarm"
                  size="sm"
                />
              </div>
              <div>
                <p class="q-my-none text-white">Duration: 6 months</p>
              </div>
            </div>
            <div class="row items-center q-mb-lg ">
              <div class="q-mr-sm">
                <q-icon
                  color="yellow"
                  name="alarm"
                  size="sm"
                />
              </div>
              <div>
                <p class="q-my-none text-white">Duration: 6 months</p>
              </div>
            </div>
            <div class="row items-center q-mb-lg ">
              <div class="q-mr-sm">
                <q-icon
                  color="yellow"
                  name="alarm"
                  size="sm"
                />
              </div>
              <div>
                <p class="q-my-none text-white">Duration: 6 months</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-1"></div>
        <div class="col q-ml-xl">

          <video
            ref="video"
            class="video-section"
            muted
            loop
            playsinline
          >
            <source src="/PersonalPortfolio-build/videos/phoneVideo.mp4" type="video/mp4" />
          </video>

        </div>
      </div>

      <!-- PROYECTO -->
      <div class="row q-mx-md q-mb-lg q-pr-xl">
        <div class="col q-ml-xl">

          <video
            ref="video"
            class="video-section"
            muted
            loop
            playsinline
          >
            <source src="/PersonalPortfolio-build/videos/phoneVideo.mp4" type="video/mp4" />
          </video>

        </div>
        <div class="col-1"></div>
        <div class="col-4">
          <!-- PROJECT NAME -->
          <div class="row inline q-gutter-sm">
            <div class=""><h5 class="txSolid q-mt-none q-mb-md">SMART</h5></div>
            <div class=""><h5 class="secondTxOutlined q-mt-none q-mb-md">ACCESS</h5></div>
          </div>
          <div class="row q-mt-sm  project-card">
            <div class="column  col justify-around q-mb-md q-ml-md">
              <div class="col ">
                <q-icon
                  name="arrow_drop_down"
                  color="purple-14"
                  size="lg"
                />
              </div>
              <div class="col">
                <q-icon
                  name="keyboard_double_arrow_right"
                  color="purple-14"
                  size="lg"
                />
              </div>
              <div class="col just">
                <h6 class="text-purple-14 q-my-none">SMART ACCESS</h6>
              </div>

            </div>
            <div class="col justify-end text-right text-yellow text-h6 content-end q-mr-md q-mb-md">01</div>
          </div>
          <!-- DESCRIPTION  -->
          <div class="text-justify text-white q-mt-md">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolor eaque id iure nostrum odit possimus
              quisquam quos voluptate? Dolor ex mollitia, nam numquam praesentium quaerat reiciendis rem similique! A
              accusamus, animi aperiam at cumque delectus distinctio dolorem est eum eveniet fuga id, ipsum, itaque
              laboriosam maiores obcaecati placeat quia veritatis</p>
          </div>
          <!-- EXTRA DATA -->
          <div class="">
            <div class="row items-center q-mb-lg ">
              <div class="q-mr-sm">
                <q-icon
                  color="yellow"
                  name="alarm"
                  size="sm"
                />
              </div>
              <div>
                <p class="q-my-none text-white">Duration: 6 months</p>
              </div>
            </div>
            <div class="row items-center q-mb-lg ">
              <div class="q-mr-sm">
                <q-icon
                  color="yellow"
                  name="alarm"
                  size="sm"
                />
              </div>
              <div>
                <p class="q-my-none text-white">Duration: 6 months</p>
              </div>
            </div>
            <div class="row items-center q-mb-lg ">
              <div class="q-mr-sm">
                <q-icon
                  color="yellow"
                  name="alarm"
                  size="sm"
                />
              </div>
              <div>
                <p class="q-my-none text-white">Duration: 6 months</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>

