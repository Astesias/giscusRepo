<script type="module">
const echartsScript = document.createElement('script');
echartsScript.src = 'https://cdn.jsdelivr.net/npm/echarts@5.4.3/dist/echarts.min.js';
echartsScript.onload = initEcharts;
document.head.appendChild(echartsScript);

// 自动渲染页面里的 ECharts 容器
function initEcharts() {
  document.querySelectorAll('.echarts-box').forEach(el => {
    const chart = echarts.init(el);
    const option = JSON.parse(el.getAttribute('data-option'));
    chart.setOption(option);
    window.addEventListener('resize', () => chart.resize());
  });
}
</script>
