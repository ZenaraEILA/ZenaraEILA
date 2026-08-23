<svg viewBox="0 0 1200 320" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    
    <filter id="soft-glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="1.5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <linearGradient id="scan-gradient" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#000" stop-opacity="0"/>
      <stop offset="50%" stop-color="#FFF" stop-opacity="0.08"/>
      <stop offset="100%" stop-color="#000" stop-opacity="0"/>
    </linearGradient>

    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#1a1a1a" stroke-width="0.5"/>
    </pattern>
  </defs>

  <!-- Background -->
  <rect width="100%" height="100%" fill="#000"/>
  
  <!-- Grid Background -->
  <rect width="100%" height="100%" fill="url(#grid)">
    <animate attributeName="opacity" values="0.3;0.6;0.3" dur="8s" repeatCount="indefinite"/>
  </rect>

  <!-- Animated Data Streams (Vertical Lines) -->
  <g stroke="#FFF" stroke-width="1" opacity="0.15">
    <line x1="100" y1="-50" x2="100" y2="370">
      <animate attributeName="y1" values="-50;0;-50" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="y2" values="370;320;370" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.15;0.4;0.15" dur="4s" repeatCount="indefinite"/>
    </line>
    <line x1="250" y1="-50" x2="250" y2="370">
      <animate attributeName="y1" values="-50;0;-50" dur="5s" repeatCount="indefinite" begin="1s"/>
      <animate attributeName="y2" values="370;320;370" dur="5s" repeatCount="indefinite" begin="1s"/>
      <animate attributeName="opacity" values="0.1;0.35;0.1" dur="5s" repeatCount="indefinite" begin="1s"/>
    </line>
    <line x1="400" y1="-50" x2="400" y2="370">
      <animate attributeName="y1" values="-50;0;-50" dur="3.5s" repeatCount="indefinite" begin="0.5s"/>
      <animate attributeName="y2" values="370;320;370" dur="3.5s" repeatCount="indefinite" begin="0.5s"/>
      <animate attributeName="opacity" values="0.2;0.5;0.2" dur="3.5s" repeatCount="indefinite" begin="0.5s"/>
    </line>
    <line x1="600" y1="-50" x2="600" y2="370">
      <animate attributeName="y1" values="-50;0;-50" dur="6s" repeatCount="indefinite" begin="2s"/>
      <animate attributeName="y2" values="370;320;370" dur="6s" repeatCount="indefinite" begin="2s"/>
      <animate attributeName="opacity" values="0.1;0.3;0.1" dur="6s" repeatCount="indefinite" begin="2s"/>
    </line>
    <line x1="800" y1="-50" x2="800" y2="370">
      <animate attributeName="y1" values="-50;0;-50" dur="4.5s" repeatCount="indefinite" begin="1.5s"/>
      <animate attributeName="y2" values="370;320;370" dur="4.5s" repeatCount="indefinite" begin="1.5s"/>
      <animate attributeName="opacity" values="0.15;0.45;0.15" dur="4.5s" repeatCount="indefinite" begin="1.5s"/>
    </line>
    <line x1="950" y1="-50" x2="950" y2="370">
      <animate attributeName="y1" values="-50;0;-50" dur="5.5s" repeatCount="indefinite" begin="0.8s"/>
      <animate attributeName="y2" values="370;320;370" dur="5.5s" repeatCount="indefinite" begin="0.8s"/>
      <animate attributeName="opacity" values="0.1;0.3;0.1" dur="5.5s" repeatCount="indefinite" begin="0.8s"/>
    </line>
    <line x1="1100" y1="-50" x2="1100" y2="370">
      <animate attributeName="y1" values="-50;0;-50" dur="3s" repeatCount="indefinite" begin="2.5s"/>
      <animate attributeName="y2" values="370;320;370" dur="3s" repeatCount="indefinite" begin="2.5s"/>
      <animate attributeName="opacity" values="0.2;0.4;0.2" dur="3s" repeatCount="indefinite" begin="2.5s"/>
    </line>
  </g>

  <!-- Floating Particles System -->
  <g fill="#FFF" filter="url(#soft-glow)">
    <!-- Particle 1 -->
    <circle cx="150" cy="280" r="2" opacity="0.6">
      <animate attributeName="cy" values="280;220;280" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.6;0.1;0.6" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="r" values="2;3;2" dur="7s" repeatCount="indefinite"/>
    </circle>
    
    <!-- Particle 2 -->
    <circle cx="350" cy="80" r="1.5" opacity="0.4">
      <animate attributeName="cy" values="80;140;80" dur="5s" repeatCount="indefinite" begin="1s"/>
      <animate attributeName="opacity" values="0.4;0.8;0.4" dur="5s" repeatCount="indefinite" begin="1s"/>
      <animate attributeName="cx" values="350;370;350" dur="5s" repeatCount="indefinite" begin="1s"/>
    </circle>
    
    <!-- Particle 3 -->
    <circle cx="550" cy="200" r="2.5" opacity="0.7">
      <animate attributeName="cy" values="200;150;200" dur="6s" repeatCount="indefinite" begin="0.5s"/>
      <animate attributeName="opacity" values="0.7;0.2;0.7" dur="6s" repeatCount="indefinite" begin="0.5s"/>
      <animate attributeName="r" values="2.5;1.5;2.5" dur="6s" repeatCount="indefinite" begin="0.5s"/>
    </circle>
    
    <!-- Particle 4 -->
    <circle cx="750" cy="100" r="2" opacity="0.5">
      <animate attributeName="cy" values="100;180;100" dur="8s" repeatCount="indefinite" begin="2s"/>
      <animate attributeName="opacity" values="0.5;0.9;0.5" dur="8s" repeatCount="indefinite" begin="2s"/>
      <animate attributeName="cx" values="750;730;750" dur="8s" repeatCount="indefinite" begin="2s"/>
    </circle>
    
    <!-- Particle 5 -->
    <circle cx="950" cy="250" r="1.8" opacity="0.6">
      <animate attributeName="cy" values="250;190;250" dur="4.5s" repeatCount="indefinite" begin="1.5s"/>
      <animate attributeName="opacity" values="0.6;0.2;0.6" dur="4.5s" repeatCount="indefinite" begin="1.5s"/>
    </circle>
    
    <!-- Particle 6 -->
    <circle cx="1050" cy="120" r="2.2" opacity="0.8">
      <animate attributeName="cy" values="120;80;120" dur="6.5s" repeatCount="indefinite" begin="0.8s"/>
      <animate attributeName="opacity" values="0.8;0.3;0.8" dur="6.5s" repeatCount="indefinite" begin="0.8s"/>
      <animate attributeName="r" values="2.2;3;2.2" dur="6.5s" repeatCount="indefinite" begin="0.8s"/>
    </circle>

    <!-- Particle 7 -->
    <circle cx="200" cy="150" r="1.2" opacity="0.3">
      <animate attributeName="cy" values="150;110;150" dur="5s" repeatCount="indefinite" begin="3s"/>
      <animate attributeName="opacity" values="0.3;0.7;0.3" dur="5s" repeatCount="indefinite" begin="3s"/>
    </circle>

    <!-- Particle 8 -->
    <circle cx="850" cy="280" r="1.8" opacity="0.5">
      <animate attributeName="cy" values="280;240;280" dur="7.5s" repeatCount="indefinite" begin="2.2s"/>
      <animate attributeName="opacity" values="0.5;0.1;0.5" dur="7.5s" repeatCount="indefinite" begin="2.2s"/>
    </circle>
  </g>

  <!-- Horizontal Scanning Lines (CRT Effect) -->
  <g>
    <rect x="0" y="0" width="1200" height="4" fill="url(#scan-gradient)" opacity="0.3">
      <animate attributeName="y" values="-10;320;-10" dur="10s" repeatCount="indefinite"/>
    </rect>
    <rect x="0" y="0" width="1200" height="3" fill="#FFF" opacity="0.06">
      <animate attributeName="y" values="-10;320;-10" dur="7s" repeatCount="indefinite" begin="3s"/>
    </rect>
    <rect x="0" y="0" width="1200" height="5" fill="url(#scan-gradient)" opacity="0.2">
      <animate attributeName="y" values="-10;320;-10" dur="12s" repeatCount="indefinite" begin="5s"/>
    </rect>
  </g>

  <!-- Corner Brackets (Animated) -->
  <g stroke="#FFF" stroke-width="1.5" fill="none" opacity="0.6">
    <!-- Top Left -->
    <path d="M 80 60 L 80 80 L 100 80">
      <animate attributeName="opacity" values="0.6;1;0.6" dur="3s" repeatCount="indefinite"/>
    </path>
    <!-- Top Right -->
    <path d="M 1120 60 L 1120 80 L 1100 80">
      <animate attributeName="opacity" values="0.6;1;0.6" dur="3s" repeatCount="indefinite" begin="0.5s"/>
    </path>
    <!-- Bottom Left -->
    <path d="M 80 260 L 80 240 L 100 240">
      <animate attributeName="opacity" values="0.6;1;0.6" dur="3s" repeatCount="indefinite" begin="1s"/>
    </path>
    <!-- Bottom Right -->
    <path d="M 1120 260 L 1120 240 L 1100 240">
      <animate attributeName="opacity" values="0.6;1;0.6" dur="3s" repeatCount="indefinite" begin="1.5s"/>
    </path>
  </g>

  <!-- Decorative Horizontal Lines -->
  <g stroke="#333" stroke-width="1">
    <line x1="150" y1="160" x2="450" y2="160">
      <animate attributeName="x1" values="150;200;150" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="450;400;450" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0.8;0.3" dur="4s" repeatCount="indefinite"/>
    </line>
    <line x1="750" y1="160" x2="1050" y2="160">
      <animate attributeName="x1" values="750;800;750" dur="4s" repeatCount="indefinite" begin="2s"/>
      <animate attributeName="x2" values="1050;1000;1050" dur="4s" repeatCount="indefinite" begin="2s"/>
      <animate attributeName="opacity" values="0.3;0.8;0.3" dur="4s" repeatCount="indefinite" begin="2s"/>
    </line>
  </g>

  <!-- Main Title -->
  <text x="600" y="155" font-family="'Courier New', monospace" font-size="52" fill="#FFF" 
        text-anchor="middle" font-weight="bold" letter-spacing="12" filter="url(#glow)">
    SERAVIEL
    <animate attributeName="opacity" values="0.85;1;0.85" dur="4s" repeatCount="indefinite"/>
  </text>

  <!-- Subtitle -->
  <text x="600" y="190" font-family="'Courier New', monospace" font-size="14" fill="#888" 
        text-anchor="middle" letter-spacing="6">
    PIXEL JURASSIC DEVELOPER
    <animate attributeName="opacity" values="0.5;0.9;0.5" dur="5s" repeatCount="indefinite"/>
  </text>

  <!-- Status Indicator -->
  <g transform="translate(600, 220)">
    <circle cx="-80" cy="0" r="3" fill="#FFF">
      <animate attributeName="opacity" values="1;0.2;1" dur="2s" repeatCount="indefinite"/>
    </circle>
    <text x="-70" y="4" font-family="'Courier New', monospace" font-size="11" fill="#666" text-anchor="start">
      SYSTEM ONLINE
    </text>
  </g>

  <!-- Bottom Decorative Line -->
  <line x1="500" y1="250" x2="700" y2="250" stroke="#222" stroke-width="1">
    <animate attributeName="stroke" values="#222;#555;#222" dur="6s" repeatCount="indefinite"/>
  </line>
</svg>
