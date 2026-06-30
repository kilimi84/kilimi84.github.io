---
layout: default
---

<section class="intro">
  <p class="name-sub">이기림 · Lee Girim</p>
  <p class="bio">
    자산운용사에서 전략기획을 합니다.<br>
    퇴근 후엔 Python으로 뭔가를 만들고,<br>
    가끔 투자를 고민하고, 드물게 여행을 갑니다.
  </p>
</section>

<hr>

<section class="post-list">
  {% if site.posts.size == 0 %}
    <p class="empty">아직 쓴 글이 없어요. 첫 글을 올려보세요.</p>
  {% endif %}
  {% for post in site.posts %}
  <a class="post-item" href="{{ post.url | relative_url }}">
    <span class="post-item-date">{{ post.date | date: "%Y.%m.%d" }}</span>
    <span class="post-item-title">{{ post.title }}</span>
  </a>
  {% endfor %}
</section>
