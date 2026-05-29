const mermaidScript = document.createElement('script');
mermaidScript.src = 'https://cdn.jsdelivr.net/npm/mermaid@11/dist/mermaid.min.js';
mermaidScript.onload = () => {
  mermaid.initialize({ startOnLoad: true, theme: 'default' });
};
document.head.appendChild(mermaidScript);
