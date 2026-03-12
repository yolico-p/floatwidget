<!-- 全局动画与样式定义 GitHub原生全支持 -->
<style>
/* 全局霓虹呼吸动画 */
@keyframes neonBreath {
  0% { text-shadow: 0 0 10px rgba(0, 229, 255, 0.5), 0 0 20px rgba(0, 229, 255, 0.3); }
  50% { text-shadow: 0 0 20px rgba(0, 229, 255, 0.9), 0 0 40px rgba(0, 128, 255, 0.6), 0 0 60px rgba(98, 0, 234, 0.4); }
  100% { text-shadow: 0 0 10px rgba(0, 229, 255, 0.5), 0 0 20px rgba(0, 229, 255, 0.3); }
}
/* 边框扫描动画 */
@keyframes scanLine {
  0% { background-position: 0 0; }
  100% { background-position: 0 200px; }
}
/* 光轨扫描动画 */
@keyframes lightTrack {
  0% { left: -100%; }
  100% { left: 100%; }
}
/* 卡片悬浮动画 */
@keyframes cardFloat {
  0% { transform: translateY(0); }
  100% { transform: translateY(-6px); }
}
/* 渐变滚动动画 */
@keyframes gradientShift {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

/* 全局样式 */
.neo-gradient {
  background: linear-gradient(135deg, #00e5ff 0%, #0080ff 50%, #6200ea 100%);
  background-size: 200% 200%;
  animation: gradientShift 4s ease infinite;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.neon-border {
  position: relative;
  border: 1px solid transparent;
  border-radius: 8px;
  background-clip: padding-box;
}
.neon-border::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  border-radius: 8px;
  background: linear-gradient(135deg, #00e5ff, #0080ff, #6200ea);
  z-index: -1;
  margin: -1px;
}
.scan-bg {
  background: linear-gradient(180deg, transparent 0%, rgba(0, 229, 255, 0.1) 50%, transparent 100%);
  background-size: 100% 200px;
  animation: scanLine 2s linear infinite;
}
.glass-card {
  background: rgba(10, 15, 30, 0.45);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(0, 229, 255, 0.2);
  border-radius: 10px;
  transition: all 0.3s ease;
}
.glass-card:hover {
  transform: translateY(-6px);
  border-color: rgba(0, 229, 255, 0.6);
  box-shadow: 0 10px 30px rgba(0, 128, 255, 0.2);
}
</style>

<!-- 全局背景 明日方舟同款深黑蓝科技网格 -->
<div style="background-color: #05070f; background-image: 
    linear-gradient(rgba(0, 229, 255, 0.03) 1px, transparent 1px),
    linear-gradient(90deg, rgba(0, 229, 255, 0.03) 1px, transparent 1px);
  background-size: 30px 30px;
  padding: 2rem 1rem;
  margin: -1rem;
  border-radius: 8px;">

<!-- 主标题区 明日方舟官网同款霓虹主视觉 -->
<div align="center">
  <h1 class="neo-gradient" style="font-size: 4.2rem; font-weight: 900; margin-bottom: 0.6rem; letter-spacing: 0.3rem; animation: neonBreath 3s ease-in-out infinite, gradientShift 4s ease infinite;">
    WINFLOAT WIDGET
  </h1>
  <h3 style="color: #c0d6f7; margin-top: 0; font-weight: 300; letter-spacing: 0.15rem; font-size: 1.2rem;">
    Windows 桌面悬浮窗解决方案 | 基于 Qt5 开发 | v1.0 稳定版
  </h3>

  <!-- 科技感徽章栏 带发光效果 -->
  <div style="margin: 2rem 0; display: flex; gap: 1rem; flex-wrap: wrap; justify-content: center;">
    <img src="https://img.shields.io/badge/Platform-Windows%2010%2F11-05070f?style=for-the-badge&logo=windows&logoColor=00e5ff&labelColor=0a0f1f" alt="平台支持" style="border: 1px solid #00e5ff; border-radius: 6px; box-shadow: 0 0 15px rgba(0, 229, 255, 0.2);">
    <img src="https://img.shields.io/badge/Framework-Qt5-05070f?style=for-the-badge&logo=qt&logoColor=41cd52&labelColor=0a0f1f" alt="开发框架" style="border: 1px solid #41cd52; border-radius: 6px; box-shadow: 0 0 15px rgba(65, 205, 82, 0.2);">
    <img src="https://img.shields.io/badge/Version-1.0-05070f?style=for-the-badge&logo=github&logoColor=0080ff&labelColor=0a0f1f" alt="当前版本" style="border: 1px solid #0080ff; border-radius: 6px; box-shadow: 0 0 15px rgba(0, 128, 255, 0.2);">
    <img src="https://img.shields.io/badge/Author-YoLiCo-05070f?style=for-the-badge&logo=codeium&logoColor=6200ea&labelColor=0a0f1f" alt="开发作者" style="border: 1px solid #6200ea; border-radius: 6px; box-shadow: 0 0 15px rgba(98, 0, 234, 0.2);">
  </div>
</div>

<!-- 科技光轨分割线 明日方舟同款数据流效果 -->
<div style="height: 2px; width: 100%; background: linear-gradient(90deg, transparent 0%, rgba(0, 229, 255, 0.5) 50%, transparent 100%); margin: 3rem 0; position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; height: 100%; width: 30%; background: linear-gradient(90deg, transparent, #ffffff, transparent); animation: lightTrack 3s ease-in-out infinite;"></div>
</div>

<!-- 📸 软件预览区 终端屏幕效果 完整截图占位 -->
<div align="center">
  <h2 class="neo-gradient" style="font-size: 2rem; font-weight: 700; letter-spacing: 0.1rem; margin-bottom: 2rem;">
    软件预览
  </h2>

  <!-- 主预览终端 带扫描线动画 明日方舟同款屏幕效果 -->
  <div class="neon-border" style="max-width: 950px; width: 100%; margin: 0 auto; padding: 5px; box-shadow: 0 0 40px rgba(0, 128, 255, 0.3);">
    <div style="position: relative; border-radius: 6px; overflow: hidden; background: #0a0f1f;">
      <!-- 屏幕顶部状态栏 -->
      <div style="height: 28px; background: linear-gradient(90deg, #0a0f1f 0%, #0f1a35 100%); display: flex; align-items: center; padding: 0 1rem; border-bottom: 1px solid rgba(0, 229, 255, 0.3);">
        <div style="display: flex; gap: 0.5rem;">
          <div style="width: 10px; height: 10px; border-radius: 50%; background: #ff5f57;"></div>
          <div style="width: 10px; height: 10px; border-radius: 50%; background: #ffbd2e;"></div>
          <div style="width: 10px; height: 10px; border-radius: 50%; background: #28ca42;"></div>
        </div>
        <span style="color: #00e5ff; margin-left: 1rem; font-size: 0.8rem; letter-spacing: 0.05rem;">WinFloat Widget v1.0 主界面</span>
      </div>
      <!-- 截图区域 带扫描线 -->
      <div style="position: relative;">
        <img src="https://via.placeholder.com/950x530/0a0f1f/00e5ff?text=WinFloat+Widget+%E4%B8%BB%E7%95%8C%E7%95%8C%E9%9D%A2%E5%AE%9E%E9%99%8C%E6%88%AA%E5%9B%BE" alt="软件主界面预览图" style="width: 100%; display: block;">
        <div class="scan-bg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none;"></div>
      </div>
    </div>
  </div>

  <br>

  <!-- 功能截图网格 三列终端卡片 -->
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(290px, 1fr)); gap: 1.5rem; max-width: 950px; margin: 0 auto;">
    <!-- 功能截图1 -->
    <div class="neon-border" style="padding: 3px; box-shadow: 0 0 20px rgba(0, 128, 255, 0.2);">
      <div style="position: relative; border-radius: 4px; overflow: hidden;">
        <img src="https://via.placeholder.com/290x170/0a0f1f/0080ff?text=自定义文字悬浮" alt="自定义文字悬浮功能截图" style="width: 100%; display: block;">
        <div class="scan-bg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none;"></div>
      </div>
    </div>
    <!-- 功能截图2 -->
    <div class="neon-border" style="padding: 3px; box-shadow: 0 0 20px rgba(0, 128, 255, 0.2);">
      <div style="position: relative; border-radius: 4px; overflow: hidden;">
        <img src="https://via.placeholder.com/290x170/0a0f1f/0080ff?text=图片悬浮适配" alt="图片悬浮适配功能截图" style="width: 100%; display: block;">
        <div class="scan-bg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none;"></div>
      </div>
    </div>
    <!-- 功能截图3 -->
    <div class="neon-border" style="padding: 3px; box-shadow: 0 0 20px rgba(0, 128, 255, 0.2);">
      <div style="position: relative; border-radius: 4px; overflow: hidden;">
        <img src="https://via.placeholder.com/290x170/0a0f1f/0080ff?text=多屏环境适配" alt="多屏环境适配功能截图" style="width: 100%; display: block;">
        <div class="scan-bg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none;"></div>
      </div>
    </div>
  </div>
  <p style="color: #889fc0; font-size: 0.9rem; margin-top: 1.5rem;">* 此处可替换为项目实际截图、演示GIF，终端样式自动适配</p>
</div>

<!-- 科技光轨分割线 -->
<div style="height: 2px; width: 100%; background: linear-gradient(90deg, transparent 0%, rgba(0, 128, 255, 0.5) 50%, transparent 100%); margin: 3rem 0; position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; height: 100%; width: 30%; background: linear-gradient(90deg, transparent, #ffffff, transparent); animation: lightTrack 3s ease-in-out infinite; animation-delay: 0.5s;"></div>
</div>

<!-- 📖 项目介绍 玻璃拟态卡片 -->
<div>
  <h2 class="neo-gradient" style="font-size: 2rem; font-weight: 700; letter-spacing: 0.1rem; text-align: center; margin-bottom: 1.5rem;">
    项目介绍
  </h2>
  <div class="glass-card" style="padding: 2rem; margin: 0 auto; max-width: 1000px;">
    <p style="color: #c0d6f7; line-height: 1.8; font-size: 1.1rem; margin: 0;">
      WinFloat Widget 是一款专为 Windows 平台打造的轻量级桌面悬浮窗工具，基于 Qt5 框架原生开发，兼顾稳定性与轻量化。
      软件支持自定义文字、图片的桌面悬浮显示，提供窗口自由拖拽、位置锁定、开机自启等核心能力，同时内置智能分辨率适配、多屏环境兼容机制，默认限制图片最大尺寸为多屏中最小屏幕分辨率的80%，从根源避免“赛博灯泡”式的视觉干扰，为用户提供简洁、稳定、高度自定义的桌面悬浮解决方案。
    </p>
  </div>
</div>

<!-- 科技光轨分割线 -->
<div style="height: 2px; width: 100%; background: linear-gradient(90deg, transparent 0%, rgba(98, 0, 234, 0.5) 50%, transparent 100%); margin: 3rem 0; position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; height: 100%; width: 30%; background: linear-gradient(90deg, transparent, #ffffff, transparent); animation: lightTrack 3s ease-in-out infinite; animation-delay: 1s;"></div>
</div>

<!-- ✨ 功能特性 玻璃拟态悬浮卡片网格 -->
<div>
  <h2 class="neo-gradient" style="font-size: 2rem; font-weight: 700; letter-spacing: 0.1rem; text-align: center; margin-bottom: 2rem;">
    功能特性
  </h2>
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(330px, 1fr)); gap: 1.8rem; max-width: 1100px; margin: 0 auto;">
    <!-- 功能卡片1 -->
    <div class="glass-card" style="padding: 1.6rem;">
      <h3 style="color: #00e5ff; margin-top: 0; display: flex; align-items: center; gap: 0.8rem; font-size: 1.25rem;">
        <span>📝</span> 自定义内容悬浮
      </h3>
      <p style="color: #a8c0e0; line-height: 1.7; margin: 0.8rem 0 0 0;">
        支持自定义文字内容与图片素材的桌面悬浮显示，可自由配置展示内容，适配各类桌面美化与信息展示需求。
      </p>
    </div>
    <!-- 功能卡片2 -->
    <div class="glass-card" style="padding: 1.6rem;">
      <h3 style="color: #00e5ff; margin-top: 0; display: flex; align-items: center; gap: 0.8rem; font-size: 1.25rem;">
        <span>🖱️</span> 窗口全维度控制
      </h3>
      <p style="color: #a8c0e0; line-height: 1.7; margin: 0.8rem 0 0 0;">
        支持悬浮窗自由拖拽位移、一键锁定/解锁窗口位置，自动记忆并恢复上次关闭前的坐标，无需重复调整布局。
      </p>
    </div>
    <!-- 功能卡片3 -->
    <div class="glass-card" style="padding: 1.6rem;">
      <h3 style="color: #00e5ff; margin-top: 0; display: flex; align-items: center; gap: 0.8rem; font-size: 1.25rem;">
        <span>⚡</span> 开机自启与状态记忆
      </h3>
      <p style="color: #a8c0e0; line-height: 1.7; margin: 0.8rem 0 0 0;">
        原生支持 Windows 开机自启，开机后自动恢复上次的悬浮窗配置、内容与位置，开箱即用无需二次设置。
      </p>
    </div>
    <!-- 功能卡片4 -->
    <div class="glass-card" style="padding: 1.6rem;">
      <h3 style="color: #00e5ff; margin-top: 0; display: flex; align-items: center; gap: 0.8rem; font-size: 1.25rem;">
        <span>🖥️</span> 多屏环境全适配
      </h3>
      <p style="color: #a8c0e0; line-height: 1.7; margin: 0.8rem 0 0 0;">
        全场景兼容多屏显示环境，可跨屏自由放置悬浮窗，精准识别多屏分辨率参数，完美适配各类多屏办公、娱乐场景。
      </p>
    </div>
    <!-- 功能卡片5 -->
    <div class="glass-card" style="padding: 1.6rem;">
      <h3 style="color: #00e5ff; margin-top: 0; display: flex; align-items: center; gap: 0.8rem; font-size: 1.25rem;">
        <span>💡</span> 智能比例与防干扰
      </h3>
      <p style="color: #a8c0e0; line-height: 1.7; margin: 0.8rem 0 0 0;">
        自动计算屏幕分辨率并适配显示比例，内置图片尺寸限制机制，从根源避免超大图片造成的“赛博灯泡”视觉干扰。
      </p>
    </div>
    <!-- 功能卡片6 -->
    <div class="glass-card" style="padding: 1.6rem;">
      <h3 style="color: #00e5ff; margin-top: 0; display: flex; align-items: center; gap: 0.8rem; font-size: 1.25rem;">
        <span>🔧</span> 轻量原生稳定运行
      </h3>
      <p style="color: #a8c0e0; line-height: 1.7; margin: 0.8rem 0 0 0;">
        基于 Qt5 框架原生开发，占用系统资源极低，后台静默稳定运行无卡顿，全量兼容 Windows 10/11 操作系统。
      </p>
    </div>
  </div>
</div>

<!-- 科技光轨分割线 -->
<div style="height: 2px; width: 100%; background: linear-gradient(90deg, transparent 0%, rgba(0, 128, 255, 0.5) 50%, transparent 100%); margin: 3rem 0; position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; height: 100%; width: 30%; background: linear-gradient(90deg, transparent, #ffffff, transparent); animation: lightTrack 3s ease-in-out infinite; animation-delay: 0.5s;"></div>
</div>

<!-- 🚧 开发计划 玻璃拟态面板 -->
<div>
  <h2 class="neo-gradient" style="font-size: 2rem; font-weight: 700; letter-spacing: 0.1rem; text-align: center; margin-bottom: 1.5rem;">
    开发计划
  </h2>
  <div class="glass-card" style="padding: 2rem; margin: 0 auto; max-width: 1000px;">
    <ul style="color: #c0d6f7; line-height: 2; font-size: 1.1rem; margin: 0; padding-left: 1.5rem;">
      <li style="margin: 0.7rem 0;">[ 开发中 ] 视频悬浮播放功能，支持本地视频循环悬浮播放与音量控制</li>
      <li style="margin: 0.7rem 0;">[ 规划中 ] 富文本内容展示支持，实现丰富的文字排版、样式与链接自定义</li>
      <li style="margin: 0.7rem 0;">[ 规划中 ] 悬浮窗透明度、层级优先级、点击穿透自定义功能</li>
      <li style="margin: 0.7rem 0;">[ 规划中 ] 更多自定义美化模板、动态特效与主题配色支持</li>
    </ul>
  </div>
</div>

<!-- 科技光轨分割线 -->
<div style="height: 2px; width: 100%; background: linear-gradient(90deg, transparent 0%, rgba(98, 0, 234, 0.5) 50%, transparent 100%); margin: 3rem 0; position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; height: 100%; width: 30%; background: linear-gradient(90deg, transparent, #ffffff, transparent); animation: lightTrack 3s ease-in-out infinite; animation-delay: 1s;"></div>
</div>

<!-- 📦 安装使用指南 玻璃拟态步骤面板 -->
<div>
  <h2 class="neo-gradient" style="font-size: 2rem; font-weight: 700; letter-spacing: 0.1rem; text-align: center; margin-bottom: 1.5rem;">
    安装使用指南
  </h2>
  <div class="glass-card" style="padding: 2rem; margin: 0 auto; max-width: 1000px;">
    <ol style="color: #c0d6f7; line-height: 2; font-size: 1.1rem; margin: 0; padding-left: 1.5rem;">
      <li style="margin: 0.8rem 0;">前往本仓库 <span style="color: #00e5ff; font-weight: 700;">Release</span> 页面，下载最新版本的安装包/便携压缩包</li>
      <li style="margin: 0.8rem 0;">便携版：解压压缩包至任意非中文路径，双击运行 <span style="color: #00e5ff; font-weight: 700;">WinFloatWidget.exe</span> 即可启动</li>
      <li style="margin: 0.8rem 0;">安装版：运行安装程序，按照指引完成安装，安装完成后自动创建桌面快捷方式</li>
      <li style="margin: 0.8rem 0;">启动软件后，右键点击系统托盘图标，即可打开设置面板，自定义悬浮内容与相关参数</li>
      <li style="margin: 0.8rem 0;">如需开机自启，在设置面板中勾选「开机自动启动」选项即可完成配置</li>
    </ol>
  </div>
</div>

<!-- 科技光轨分割线 -->
<div style="height: 2px; width: 100%; background: linear-gradient(90deg, transparent 0%, rgba(0, 229, 255, 0.5) 50%, transparent 100%); margin: 3rem 0; position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; height: 100%; width: 30%; background: linear-gradient(90deg, transparent, #ffffff, transparent); animation: lightTrack 3s ease-in-out infinite;"></div>
</div>

<!-- 📜 许可证 双列玻璃拟态面板 -->
<div>
  <h2 class="neo-gradient" style="font-size: 2rem; font-weight: 700; letter-spacing: 0.1rem; text-align: center; margin-bottom: 1.5rem;">
    许可证
  </h2>
  <div class="glass-card" style="padding: 2rem; margin: 0 auto; max-width: 1000px;">
    <p style="color: #c0d6f7; line-height: 1.7; margin: 0 0 1.5rem 0; font-size: 1.05rem;">
      本项目采用 <span style="color: #00e5ff; font-weight: 700;">自定义非商用专属许可证</span>，使用本软件即视为您同意以下核心条款，完整协议内容详见仓库内 <a href="LICENSE" style="color: #00e5ff; text-decoration: underline;">LICENSE</a> 文件。
    </p>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); gap: 1.5rem; margin-top: 1rem;">
      <!-- 许可范围 -->
      <div style="border: 1px solid rgba(0, 229, 255, 0.4); border-radius: 8px; padding: 1.5rem; background: rgba(0, 229, 255, 0.05);">
        <h4 style="color: #00e5ff; margin-top: 0; margin-bottom: 1rem; font-size: 1.2rem;">✅ 许可范围</h4>
        <ul style="color: #a8c0e0; line-height: 1.8; margin: 0; padding-left: 1.2rem;">
          <li>个人非商业用途的安装、使用</li>
          <li>无修改的原始版本复制与分发</li>
        </ul>
      </div>
      <!-- 禁止行为 -->
      <div style="border: 1px solid rgba(255, 71, 87, 0.4); border-radius: 8px; padding: 1.5rem; background: rgba(255, 71, 87, 0.05);">
        <h4 style="color: #ff4757; margin-top: 0; margin-bottom: 1rem; font-size: 1.2rem;">❌ 禁止行为</h4>
        <ul style="color: #a8c0e0; line-height: 1.8; margin: 0; padding-left: 1.2rem;">
          <li>任何形式的商业用途与盈利行为</li>
          <li>私自二次修改、反编译、二次分发</li>
          <li>对本软件进行收费、捆绑分发</li>
          <li>去除或修改软件内的版权声明与标识</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<!-- 科技光轨分割线 -->
<div style="height: 2px; width: 100%; background: linear-gradient(90deg, transparent 0%, rgba(98, 0, 234, 0.5) 50%, transparent 100%); margin: 3rem 0; position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; height: 100%; width: 30%; background: linear-gradient(90deg, transparent, #ffffff, transparent); animation: lightTrack 3s ease-in-out infinite; animation-delay: 1s;"></div>
</div>

<!-- 👤 关于作者 沉浸式霓虹面板 -->
<div align="center">
  <h2 class="neo-gradient" style="font-size: 2rem; font-weight: 700; letter-spacing: 0.1rem; margin-bottom: 2rem;">
    关于作者
  </h2>
  <div class="neon-border" style="max-width: 700px; width: 100%; margin: 0 auto; padding: 6px; box-shadow: 0 0 40px rgba(98, 0, 234, 0.3);">
    <div style="background: linear-gradient(135deg, rgba(0, 229, 255, 0.08) 0%, rgba(98, 0, 234, 0.08) 100%); border-radius: 8px; padding: 2.5rem; backdrop-filter: blur(10px); -webkit-backdrop-filter: blur(10px);">
      <h3 class="neo-gradient" style="font-size: 2.2rem; font-weight: 800; margin: 0 0 1rem 0; letter-spacing: 0.1rem;">
        柚柠可 | YoLiCo
      </h3>
      <p style="color: #a8c0e0; line-height: 1.7; margin: 0 0 2rem 0; font-size: 1.1rem;">
        本项目由 柚柠可(YoLiCo) 独立开发与维护
      </p>
      <div style="display: flex; justify-content: center; gap: 1.5rem; flex-wrap: wrap;">
        <a href="https://yolico.net" target="_blank" style="background: linear-gradient(135deg, #0080ff, #00e5ff); color: #fff; padding: 0.9rem 2rem; border-radius: 6px; text-decoration: none; font-weight: 600; font-size: 1rem; box-shadow: 0 0 20px rgba(0, 128, 255, 0.4); transition: all 0.3s ease;">
          个人主页
        </a>
        <a href="https://world.yolico.net" target="_blank" style="background: linear-gradient(135deg, #6200ea, #9d4edd); color: #fff; padding: 0.9rem 2rem; border-radius: 6px; text-decoration: none; font-weight: 600; font-size: 1rem; box-shadow: 0 0 20px rgba(98, 0, 234, 0.4); transition: all 0.3s ease;">
          小世界 | 个人博客
        </a>
      </div>
    </div>
  </div>
</div>

<!-- 科技光轨分割线 -->
<div style="height: 2px; width: 100%; background: linear-gradient(90deg, transparent 0%, rgba(0, 229, 255, 0.5) 50%, transparent 100%); margin: 3rem 0; position: relative; overflow: hidden;">
  <div style="position: absolute; top: 0; left: 0; height: 100%; width: 30%; background: linear-gradient(90deg, transparent, #ffffff, transparent); animation: lightTrack 3s ease-in-out infinite;"></div>
</div>

<!-- 底部版权 -->
<div align="center">
  <p class="neo-gradient" style="font-size: 0.95rem; line-height: 1.8; font-weight: 500; letter-spacing: 0.05rem;">
    Copyright © 2026 柚柠可(YoLiCo). All Rights Reserved.<br>
    本项目最终解释权归作者所有
  </p>
</div>

</div>