---
layout: uikit-single
title: Navigation
slug: navigation
draft: true
publishDate: 2024-10-10
tags:
  - ui-kit
---

<script setup lang="ts">
</script>


<nav class="paginav">
              <a
                :title="'some title 1'"
                class="prev"
              >
                <span class="title">« Предыдущие видео</span>
                <br>
                <span>some title 1</span>
              </a>
              <a
                :title="'some title 2'"
                class="next"
              >
                <span class="title">Следующие видео »</span>
                <br>
                <span>some title 2</span>
              </a>
            </nav>


#### If there is no prev:


<nav class="paginav">
              <a
                class="prev is--disabled"
              >&nbsp;</a>
              <a
                :title="'some title 2'"
                class="next"
              >
                <span class="title">Следующие видео »</span>
                <br>
                <span>some title 2</span>
              </a>
            </nav>