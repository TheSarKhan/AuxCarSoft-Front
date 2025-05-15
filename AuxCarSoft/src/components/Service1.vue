<script setup>
import { themeColor } from "../data/items";
import personPhoto from "../assets/images/person_1.jpg";
import mainPhoto from "../assets/images/service1.jpg";

const service1Heading = "Digital Services";
const service1SubHeading = "Selling Digital Services";
const service1Quote =
  '"With AuxCarSoft’s tools, we gained full visibility into our auction shipments and improved our logistics workflow dramatically."';
const personName = "James Anderson";
const designation = "Facebook, Product Lead";
function youtubeVideoUrl() {
  const youtubeVideoId = "FzRH7y3LbQE";
  return `https://www.youtube.com/watch?v=${youtubeVideoId}&amp;t=9s`;
}
</script>
<template>
  <div class="untree_co-section" id="features-section">
    <div class="container">
      <div class="row justify-content-between">
        <div class="col-lg-4">
          <span
            class="caption"
            data-aos="fade-up"
            data-aos-delay="0"
            :style="[{ color: themeColor }]"
            >{{ service1Heading }}</span
          >
          <h3 class="heading mb-4" data-aos="fade-up" data-aos-delay="100">
            {{ service1SubHeading }}
          </h3>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="200">
            <p>
              We deliver tailored digital solutions for logistics firms importing auctioned vehicles. Our services include CRM systems, auction tracking software, custom websites, and real-time dashboards—designed to streamline operations and boost efficiency.
            </p>
            <ul class="list-unstyled ul-check primary">
              <li>Fast</li>
              <li>Professional</li>
            </ul>
          </div>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="300">
            <div class="untree_co-testimonial d-flex">
              <div class="text">
                <blockquote>
                  {{ service1Quote }}
                </blockquote>
                <div class="author d-flex">
                  <div class="pic mr-3">
                    <img :src="personPhoto" alt="Image" class="img-fluid" />
                  </div>
                  <div>
                    <strong class="d-block">{{ personName }}</strong
                    ><span class="d-block">{{ designation }}</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-7" data-aos="fade-up" data-aos-delay="400">
          <a :href="youtubeVideoUrl()" class="btn-video" data-fancybox>
            <span class="wrap-icon-play">
              <svg
                class="bi bi-play-fill"
                width="1em"
                height="1em"
                viewBox="0 0 16 16"
                fill="currentColor"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M11.596 8.697l-6.363 3.692c-.54.313-1.233-.066-1.233-.697V4.308c0-.63.692-1.01 1.233-.696l6.363 3.692a.802.802 0 0 1 0 1.393z"
                />
              </svg>
            </span>
            <img :src="mainPhoto" alt="Image" class="img-fluid img-shadow" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
