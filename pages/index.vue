<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-xs-12 text-align-center">
          <a href="/images/foto-note.jpg" target="_blank" class="image-container">
            <img
              class="hero-image centered-image"
              src="/images/foto-note.jpg"
              title="Antonio Henrique Machado"
            />
          </a>
          <h1 class="hero-title">Antonio Henrique Machado</h1>
          <div class="hero-description">
            <p>
              Apaixonado por <strong>Tecnologia</strong> e <strong>Pessoas</strong>! 🤎
            </p>
          </div>

          
        </div>
      </div>

      <div class="row margin-top-2">
        <div class="col-xs-12 text-align-center">
          <div
            class="github-card"
            data-github="machadoah"
            data-width="400"
            data-height="150"
            data-theme="default"
          ></div>
          <script src="//cdn.jsdelivr.net/github-cards/latest/widget.js"></script>
          <hr class="divider" />
          <div class="hero-links">
      <a href="https://youtube.com/@ExceptionCode" class="link-box">
        <span class="emoji">📺</span>
        <span class="text">YouTube</span>
      </a>
      <a href="https://instagram.com/machadoah" class="link-box">
        <span class="emoji">🖼️</span>
        <span class="text">Instagram</span>
      </a>
      <a href="https://linkedin.com/in/machadoah" class="link-box">
        <span class="emoji">💼</span>
        <span class="text">Linkedin</span>
      </a>
      <a href="https://github.com/machadoah" class="link-box">
        <span class="emoji">🐈‍⬛</span>
        <span class="text">Github</span>
      </a>
      <a href="https://machadoah.medium.com" class="link-box">
        <span class="emoji">📰</span>
        <span class="text">Medium</span>
      </a>
      <a href="https://dev.to/machadoah" class="link-box">
        <span class="emoji">👨🏽‍💻</span>
        <span class="text">Dev.to</span>
      </a>
    </div>
    <hr class="divider" />
          <div class="hero-links-final">
            <a href="https://keepo.io/machadoah/">Keepo</a>
            <br></br>
            <br></br>
            <br></br>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'machadoah',
      meta: [
        { hid: 'description', name: 'description', content: 'Gosto muito da área de tecnologia e estou sempre buscando estudar, e me desenvolver nessa área, sempre buscando novos conhecimentos!' },
        { property: 'og:type', content: 'website' },
        { property: 'og:locale', content: 'pt_BR' },
        { property: 'og:title', content: 'Antonio Henrique Machado' },
        { property: 'og:description', content: 'Gosto muito da área de tecnologia e estou sempre buscando estudar, e me desenvolver nessa área, sempre buscando novos conhecimentos!' },
        { property: 'og:url', content: 'https://github.com/machadoah/' },
        { property: 'og:image', content: 'https://github.com/machadoah' }
      ],
      link: [
        { rel: 'icon', type: 'image/svg+xml', href: 'data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>🪓</text></svg>' },
        { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=Merriweather:300,700|Open+Sans:700,400&subset=latin,latin-ext' }
      ],
      script: [
        { src: 'https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js', async: true },
        {
          hid: 'google-analytics',
          innerHTML: `
            (function(i,s,o,g,r,a,m) {
              i["GoogleAnalyticsObject"]=r;
              (i[r]=i[r]||function(){
                (i[r].q=i[r].q||[]).push(arguments);
              }),
              (i[r].l=1*new Date());
              (a=s.createElement(o)),
              (m=s.getElementsByTagName(o)[0]);
              a.async=1;
              a.src=g;
              m.parentNode.insertBefore(a,m);
            })(window,document,"script","//www.google-analytics.com/analytics.js","ga");
            ga("create","UA-120989-9","auto");
            ga("send","pageview");
          `,
          type: 'text/javascript',
          defer: true
        }
      ],
      __dangerouslyDisableSanitizers: ['script']
    }
  }
}
</script>
