<script setup>
import { contactInfo } from "../data/items";

const copyrightText = "Copyright 2025, All rights reserved.";
const column1Heading = "About Launch";
const column1Text =
  "We launched our platform to empower logistics companies handling auctioned vehicles. By combining innovative technology with deep industry knowledge, we help streamline operations, boost efficiency, and bring transparency to every step—from auction tracking to customer engagement.";
const column2Heading = "Projects";
const column3Heading = "Services";
const column4Heading = "Contact";

const connectHeading = "Connect";

const socialItems = [
  {
    link: "https://www.instagram.com/",
    icon: "icon-instagram",
  },
  {
    link: "https://www.twitter.com/",
    icon: "icon-twitter",
  },
  {
    link: "https://www.facebook.com/",
    icon: "icon-facebook",
  },
  {
    link: "https://www.linkedin.com/",
    icon: "icon-linkedin",
  },
  {
    link: "https://www.pinterest.com/",
    icon: "icon-pinterest",
  },
];
</script>

<template>
  <div class="site-footer">
    <div class="footer-dots"></div>
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <div class="widget">
            <h3>{{ column1Heading }}</h3>
            <p>{{ column1Text }}</p>
          </div>
          <div class="widget">
            <h3>{{ connectHeading }}</h3>
            <ul class="list-unstyled social">
              <li style="margin-right: 4px">
                <a :href="socialItems[0].link"
                  ><span :class="socialItems[0].icon"></span
                ></a>
              </li> 
              <li style="margin-right: 4px">
                <a :href="socialItems[2].link"
                  ><span :class="socialItems[2].icon"></span
                ></a>
              </li>
              <li style="margin-right: 4px">
                <a :href="socialItems[3].link"
                  ><span :class="socialItems[3].icon"></span
                ></a>
              </li> 
            </ul>
          </div>
        </div>
        <div class="col-lg-2 ml-auto">
          <div class="widget">
            <h3>{{ column2Heading }}</h3>
            <ul class="list-unstyled float-left links"> 
              <li><a href="#">Auxion Tracking</a></li>
               
            </ul>
          </div>
        </div>
        <div class="col-lg-2">
          <div class="widget">
            <h3>{{ column3Heading }}</h3>
            <ul class="list-unstyled float-left links">
              <li><a href="#">CRM Systems</a></li>
              <li><a href="#">Auction Tracking Systems</a></li>
              <li><a href="#">Website Development</a></li>
              <li><a href="#">Dashboard & Admin Panel</a></li>
            </ul>
          </div>
        </div>
        <div class="col-lg-3">
          <div class="widget">
            <h3>{{ column4Heading }}</h3>
            <address>{{ contactInfo.address }}</address>
            <ul class="list-unstyled links mb-4">
              <li>
                <a :href="'tel://' + contactInfo.phone1">{{
                  contactInfo.phone1
                }}</a>
              </li>
              <li>
                <a :href="'tel://' + contactInfo.phone2">{{
                  contactInfo.phone2
                }}</a>
              </li>
              <li>
                <a :href="'mailto:' + contactInfo.email"
                  ><span>{{ contactInfo.email }}</span></a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="row mt-5">
        <div class="col-12 text-center">
          <p>
            {{ copyrightText }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
