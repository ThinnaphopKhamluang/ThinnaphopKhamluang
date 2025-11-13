<img src="https://raw.githubusercontent.com/USERNAME/REPO/main/penguin.svg" width="320"/>
<!-- Animated Penguin for GitHub README -->
<svg xmlns="http://www.w3.org/2000/svg" width="320" height="180" viewBox="0 0 320 180" role="img" aria-label="Animated Penguin">
  <style>
    /* พื้นหลังหิมะ */
    .snow {
      fill: #e8f6ff;
    }
    .snowflake {
      animation: fall 5s linear infinite;
      opacity: 0.8;
    }
    @keyframes fall {
      0% { transform: translateY(-10px); opacity: 0.8; }
      100% { transform: translateY(180px); opacity: 0.2; }
    }

    /* การเคลื่อนไหวเพนกวิน */
    .penguin {
      animation: waddle 3.2s ease-in-out infinite;
      transform-origin: 50% 50%;
    }
    @keyframes waddle {
      0%   { transform: translateX(0) scaleX(1); }
      50%  { transform: translateX(90px) scaleX(-1); }
      100% { transform: translateX(0) scaleX(1); }
    }

    /* ปีกกระพือ */
    .wing {
      animation: flap 0.7s ease-in-out infinite;
      transform-origin: 50% 50%;
    }
    @keyframes flap {
      0% { transform: rotate(0deg); }
      50% { transform: rotate(-15deg); }
      100% { transform: rotate(0deg); }
    }

    /* กะพริบตา */
    .eye {
      animation: blink 4s steps(1) infinite;
    }
    @keyframes blink {
      0%, 95% { transform: scaleY(1); }
      96%, 100% { transform: scaleY(0.1); }
    }
  </style>

  <!-- ท้องฟ้า -->
  <rect width="100%" height="100%" class="snow"/>

  <!-- หิมะตก -->
  <circle class="snowflake" cx="30" cy="10" r="2" fill="white" style="animation-delay:0s"/>
  <circle class="snowflake" cx="100" cy="0" r="1.5" fill="white" style="animation-delay:1s"/>
  <circle class="snowflake" cx="160" cy="5" r="2.2" fill="white" style="animation-delay:2s"/>
  <circle class="snowflake" cx="230" cy="10" r="1.8" fill="white" style="animation-delay:1.5s"/>
  <circle class="snowflake" cx="280" cy="3" r="2" fill="white" style="animation-delay:2.8s"/>

  <!-- พื้นหิมะ -->
  <ellipse cx="160" cy="160" rx="160" ry="25" fill="#d3f0ff"/>

  <!-- ตัวเพนกวิน -->
  <g class="penguin" transform="translate(60,30)">
    <!-- ขา -->
    <g transform="translate(110,100)">
      <ellipse cx="-14" cy="8" rx="8" ry="4" fill="#ffad33"/>
      <ellipse cx="14" cy="8" rx="8" ry="4" fill="#ffad33"/>
    </g>

    <!-- ลำตัว -->
    <ellipse cx="110" cy="70" rx="50" ry="65" fill="#111"/>
    <ellipse cx="110" cy="78" rx="34" ry="48" fill="#fff"/>

    <!-- ปีก -->
    <g class="wing" transform="translate(60,70)">
      <path d="M0 0 C -25 8, -30 35, -5 40 C 5 42, 10 36, 6 10 Z" fill="#111"/>
    </g>
    <g class="wing" transform="translate(160,70)">
      <path d="M0 0 C 25 8, 30 35, 5 40 C -5 42, -10 36, -6 10 Z" fill="#111"/>
    </g>

    <!-- หัว -->
    <g transform="translate(110,25)">
      <circle cx="0" cy="0" r="24" fill="#111"/>
      <ellipse cx="0" cy="6" rx="16" ry="20" fill="#fff"/>
      <g transform="translate(-6,-2)">
        <ellipse class="eye" cx="0" cy="0" rx="3.5" ry="4.5" fill="#111"/>
      </g>
      <g transform="translate(6,-2)">
        <ellipse class="eye" cx="0" cy="0" rx="3.5" ry="4.5" fill="#111"/>
      </g>
      <path d="M-5 6 L0 12 L5 6 L0 8 Z" fill="#ffad33"/>
    </g>
  </g>
</svg>
