<script setup lang="ts">

import {authors, randomize} from "../utils";
import {blogs} from '../utils/data'
import Blog from "../components/Blog.vue";
</script>

<template>
  <!-- Start Page Title Section -->
  <div class="page-title-area item-bg1">
    <div class="d-table">
      <div class="d-table-cell">
        <div class="container">
          <div class="page-title-content">
            <h2>Blogs</h2>
            <ul>
              <li><router-link to="/">Home</router-link>
              </li>
              <li>Blogs</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- End Page Title Section -->

  <!-- Start Blog Section -->
  <section class="blog-section section-padding">
    <div class="container">
      <div class="row">
        <template v-for="blog in blogs" :key="blog.id">
          <div class="col-lg-4 col-md-6">
          <Blog :blog="blog"></Blog>
          </div>
        </template>

        <div class="col-lg-4 col-md-6">
          <router-link :to="'/blogs/'+randomize([1,2,3,4,5])"></router-link>
          <div class="blog-single-item">
            <div class="blog-image">
              <a href="single-blog.html">
                <img src="../assets/img/blog-1.jpg" alt="image">
              </a>
            </div>
            <div class="blog-description">
              <ul class="blog-info">
                <li>
                  <a href="#"><i class="bi bi-person-circle"></i>{{randomize(authors)}}</a>
                </li>
                <li>
                  <a href="#"><i class="bi bi-calendar-check"></i> 17 June 2024</a>
                </li>
              </ul>
              <div class="blog-text">
                <h3>
                  <a href="single-blog.html">
                    Planning for a Safe Return to the Workplace IT Solutions
                  </a>
                </h3>
                <p>Lorem ipsum dolor sit amet, consectetu adipiscing elit, sed eiusmod tempor incididunt ut labore dolore magna aliqua</p>
                <div class="blog-btn"> <a href="single-blog.html" class="read-more"><i class="bi bi-arrow-right-short"></i> Read More</a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="blog-single-item">
            <div class="blog-image">
              <a href="single-blog.html">
                <img src="../assets/img/blog-2.jpg" alt="image">
              </a>
            </div>
            <div class="blog-description">
              <ul class="blog-info">
                <li>
                  <a href="#"><i class="bi bi-person-circle"></i>{{randomize(authors)}}</a>
                </li>
                <li>
                  <a href="#"><i class="bi bi-calendar-check"></i> 20 June 2024</a>
                </li>
              </ul>
              <div class="blog-text">
                <h3>
                  <a href="single-blog.html">
                    Announcing Our New Smiles for Success Charity
                  </a>
                </h3>
                <p>Lorem ipsum dolor sit amet, consectetu adipiscing elit, sed eiusmod tempor incididunt ut labore dolore magna aliqua</p>
                <div class="blog-btn">
                  <a href="single-blog.html" class="read-more"><i class="bi bi-arrow-right-short"></i> Read More</a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="blog-single-item">
            <div class="blog-image">
              <a href="single-blog.html">
                <img src="../assets/img/blog-3.jpg" alt="image">
              </a>
            </div>
            <div class="blog-description">
              <ul class="blog-info">
                <li>
                  <a href="#"><i class="bi bi-person-circle"></i>{{randomize(authors)}}</a>
                </li>
                <li>
                  <a href="#"><i class="bi bi-calendar-check"></i> 25 June 2024</a>
                </li>
              </ul>
              <div class="blog-text">
                <h3>
                  <a href="single-blog.html">
                    Machine Learning Applications for Every Industry
                  </a>
                </h3>
                <p>Lorem ipsum dolor sit amet, consectetu adipiscing elit, sed eiusmod tempor incididunt ut labore dolore magna aliqua</p>
                <div class="blog-btn"> <a href="single-blog.html" class="read-more"><i class="bi bi-arrow-right-short"></i> Read More</a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="blog-single-item">
            <div class="blog-image">
              <a href="single-blog.html">
                <img src="../assets/img/blog-4.jpg" alt="image">
              </a>
            </div>
            <div class="blog-description">
              <ul class="blog-info">
                <li>
                  <a href="#"><i class="bi bi-person-circle"></i>{{randomize(authors)}}</a>
                </li>
                <li>
                  <a href="#"><i class="bi bi-calendar-check"></i> 27 June 2024</a>
                </li>
              </ul>
              <div class="blog-text">
                <h3>
                  <a href="single-blog.html">
                    5 Technology Considerations for Office Relocations
                  </a>
                </h3>
                <p>Lorem ipsum dolor sit amet, consectetu adipiscing elit, sed eiusmod tempor incididunt ut labore dolore magna aliqua</p>
                <div class="blog-btn"> <a href="single-blog.html" class="read-more"><i class="bi bi-arrow-right-short"></i> Read More</a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="blog-single-item">
            <div class="blog-image">
              <a href="single-blog.html">
                <img src="../assets/img/blog-5.jpg" alt="image">
              </a>
            </div>
            <div class="blog-description">
              <ul class="blog-info">
                <li>
                  <a href="#"><i class="bi bi-person-circle"></i>{{randomize(authors)}}</a>
                </li>
                <li>
                  <a href="#"><i class="bi bi-calendar-check"></i> 28 June 2024</a>
                </li>
              </ul>
              <div class="blog-text">
                <h3>
                  <a href="single-blog.html">
                    Everything you need to know about geo-blocking
                  </a>
                </h3>
                <p>Lorem ipsum dolor sit amet, consectetu adipiscing elit, sed eiusmod tempor incididunt ut labore dolore magna aliqua</p>
                <div class="blog-btn">
                  <a href="single-blog.html" class="read-more"><i class="bi bi-arrow-right-short"></i> Read More</a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="blog-single-item">
            <div class="blog-image">
              <a href="single-blog.html">
                <img src="../assets/img/blog-6.jpg" alt="image">
              </a>
            </div>
            <div class="blog-description">
              <ul class="blog-info">
                <li>
                  <a href="#"><i class="bi bi-person-circle"></i>{{randomize(authors)}}</a>
                </li>
                <li>
                  <a href="#"><i class="bi bi-calendar-check"></i> 30 June 2024</a>
                </li>
              </ul>
              <div class="blog-text">
                <h3>
                  <a href="single-blog.html">
                    Internal or outsourced IT: What’s the best choice?
                  </a>
                </h3>
                <p>Lorem ipsum dolor sit amet, consectetu adipiscing elit, sed eiusmod tempor incididunt ut labore dolore magna aliqua</p>
                <div class="blog-btn"> <a href="single-blog.html" class="read-more"><i class="bi bi-arrow-right-short"></i> Read More</a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-12 col-md-12">
          <div class="pagination-area"> <a href="#" class="prev page-numbers"><i class="fas fa-angle-left"></i></a>
            <a href="#" class="page-numbers">1</a>
            <span class="page-numbers current" aria-current="page">2</span>
            <a href="#" class="page-numbers">3</a>
            <a href="#" class="page-numbers">4</a>
            <a href="#" class="next page-numbers"><i class="fas fa-angle-right"></i></a>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- End Blog Section -->

</template>

<style scoped>

</style>
