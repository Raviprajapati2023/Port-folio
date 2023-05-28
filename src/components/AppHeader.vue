<template>
  <div class="relative">
    <main>
      <HeadingSection />
      <ImageSection />

      <!-- // image sectiion  -->
      <div class="sm:px-8 mt-24 md:mt-28">
        <div class="mx-auto max-w-7xl lg:px-8">
          <div class="relative px-4 sm:px-8 lg:px-12">
            <div class="mx-auto max-w-2xl lg:max-w-5xl">
              <div
                class="mx-auto grid max-w-xl grid-cols-1 gap-y-20 lg:max-w-none lg:grid-cols-2"
              >
                <!-- // Article Section  -->
                <ArticleSection />
                <div class="space-y-10 lg:pl-16 xl:pl-24">
                  <ContactForm />
                  <!-- // WorkComponent   -->
                  <WorkSection />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>
<script setup>
import WorkSection from "./WorkSection.vue";
import ContactForm from "./ContactForm.vue";
import ArticleSection from "./ArticleSection.vue";
import HeadingSection from "./HeadingSection.vue";
import ImageSection from "./ImageSection.vue";
</script>
