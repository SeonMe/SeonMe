<div align="center">

  <!-- 顶部动态终端窗 -->
  <svg width="600" height="140" viewBox="0 0 600 140" xmlns="http://www.w3.org/2000/svg">
    <rect x="0" y="0" width="600" height="140" rx="12" fill="#0D1117" stroke="#30363D" stroke-width="2" />
    
    <!-- 窗口按钮 -->
    <circle cx="20" cy="20" r="6" fill="#FF5F56" />
    <circle cx="40" cy="20" r="6" fill="#FFBD2E" />
    <circle cx="60" cy="20" r="6" fill="#27C93F" />
    
    <!-- 动态闪烁光标 -->
    <rect x="45" y="55" width="10" height="24" fill="#58A6FF">
      <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite" />
    </rect>
    
    <!-- 打字动画：逐渐显示的文字 -->
    <text x="45" y="73" font-family="monospace" font-size="20" fill="#58A6FF" font-weight="bold">
      <tspan>
        ./launch.sh —system
        <animate attributeName="fill-opacity" from="0" to="1" begin="0.5s" dur="0.1s" fill="freeze" />
      </tspan>
      <tspan dx="0" dy="0">
        <animate attributeName="fill-opacity" from="0" to="1" begin="0.6s" dur="0.1s" fill="freeze" />
      </tspan>
    </text>

    <!-- 第二行：身份标识 -->
    <text x="45" y="100" font-family="monospace" font-size="18" fill="#C9D1D9">
      <tspan fill-opacity="0">
        > identity: SeonMe
        <animate attributeName="fill-opacity" from="0" to="1" begin="2s" dur="0.8s" fill="freeze" />
      </tspan>
    </text>

    <!-- 第三行：系统消息 -->
    <text x="45" y="125" font-family="monospace" font-size="14" fill="#8B949E">
      <tspan fill-opacity="0">
        status: online · coffee level: critical
        <animate attributeName="fill-opacity" from="0" to="1" begin="3s" dur="0.8s" fill="freeze" />
      </tspan>
    </text>
  </svg>

  <br/>
  <br/>

  <!-- ═══ 核心终端 About Me ═══ -->
  <!-- 使用纯文本 + 一个动态 SVG 光标做点缀 -->
  <table align="center">
    <tr>
      <td>
        <pre style="background:#0D1117; color:#58A6FF; padding:20px; border-radius:12px; border:1px solid #30363D; position:relative;">
┌─────────────────────────────────────────┐
│  <b>~/about_me</b>                           │
├─────────────────────────────────────────┤
│                                         │
│  $ <b>cat</b> bio.txt                      │
│                                         │
│  > 全栈开发者，以代码为笔在数字世界绘  │
│    画的人。                              │
│  > 痴迷于 Rust 的内存安全哲学，          │
│    也用 TypeScript 构建可扩展的 web。    │
│  > 相信工具塑造思维：                  │
│    · 编辑器：Neovim                     │
│    · 系统：Arch Linux                   │
│    · Shell：Zsh + oh-my-zsh             │
│  > 大脑状态：Idea Overflow  ∞/∞        │
│                                         │
│  $ <b>echo</b> $MOTTO                     │
│  "Code is poetry that does something." │
│                                         │
│  $ <span id="blinking">█</span>                           │
└─────────────────────────────────────────┘
        </pre>
        <!-- 单独的光标 SVG 叠加在文本上，保证闪烁 -->
        <svg style="position:absolute; top:0; left:0;" width="100%" height="100%">
          <!-- 只是一个透明层，实际闪烁用 pre 内的字符即可，这里是双保险 -->
        </svg>
      </td>
    </tr>
  </table>

  <p>
    <sub>「 这个终端就是你，实时从 GitHub 读取你的灵魂 」</sub>
  </p>

  <!-- 底部动态呼吸圈 -->
  <svg width="200" height="40" viewBox="0 0 200 40" xmlns="http://www.w3.org/2000/svg">
    <circle cx="100" cy="20" r="8" fill="#58A6FF">
      <animate attributeName="r" values="8;14;8" dur="2s" repeatCount="indefinite" />
      <animate attributeName="opacity" values="1;0.5;1" dur="2s" repeatCount="indefinite" />
    </circle>
    <text x="115" y="25" font-family="monospace" font-size="12" fill="#8B949E">system activated</text>
  </svg>

</div>
