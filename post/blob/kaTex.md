<script type="module">
  // 加载 KaTeX 样式
  const link = document.createElement('link');
  link.rel = 'stylesheet';
  link.href = 'https://cdn.jsdelivr.net/npm/katex@0.16.18/dist/katex.min.css';
  document.head.appendChild(link);

  // 加载 KaTeX
  const katexScript = document.createElement('script');
  katexScript.src = 'https://cdn.jsdelivr.net/npm/katex@0.16.18/dist/katex.min.js';
  katexScript.onload = renderAllMath;
  document.head.appendChild(katexScript);

  // 加载自动渲染 $...$
  const renderScript = document.createElement('script');
  renderScript.src = 'https://cdn.jsdelivr.net/npm/katex@0.16.18/dist/contrib/auto-render.min.js';
  document.head.appendChild(renderScript);

  // 自动渲染页面所有公式
  function renderAllMath() {
    if (window.renderMathInElement) {
      renderMathInElement(document.body, {
        delimiters: [
          { left: "$$", right: "$$", display: true },
          { left: "$", right: "$", display: false }
        ]
      });
    }
  }
</script>
