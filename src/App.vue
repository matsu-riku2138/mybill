<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container">
          <a class="navbar-brand" href="/"><h2>会計.com</h2></a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
              <ul class="navbar-nav ms-auto">
                  <li class="nav-item">
                      <RouterLink class="nav-link active" to="/">ホーム</RouterLink>
                      <!-- <a class="nav-link active" href="/about">サイトについて</a> -->
                  </li>
                  <li class="nav-item">
                      <RouterLink class="nav-link active" to="/about">サイトについて</RouterLink>
                      <!-- <a class="nav-link active" href="/about">サイトについて</a> -->
                  </li>
                  <li class="nav-item">
                      <RouterLink class="nav-link active" to="/contact">お問い合わせ</RouterLink>
                      <!-- <a class="nav-link active" href="/contact">問い合わせ</a> -->
                  </li>
              </ul>
          </div>
      </div>
    </nav>
  </header>
  <main>
    <RouterView />
  </main>
  <hr>
  <footer class="footer pb-4">
    <div class="container pt-5 text-center">
        <div class="row justify-content-center pb-3">
            <div class="col">
                <div class="sns-icon-twitter float-end">
                    <a href="https://twitter.com">
                        <i class="bi bi-twitter" style="font-size:36px;color: rgb(29,155,240);"></i>
                    </a>
                </div>
            </div>
            <div class="col">
                <div class="sns-icon-github float-start">
                    <a href="https://github.com">
                        <i class="bi bi-github" style="font-size:36px; color: #000;"></i>
                    </a>
                </div>
            </div>
        </div>
        <p class="copyright">&copy;2022-2024 会計.com All Rights Reserved.</p>
    </div>
  </footer>
</template>