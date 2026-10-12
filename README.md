<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 360" width="1200" height="360" role="img" aria-label="Astronauta flutuando no espaço">
  <defs>
    <linearGradient id="sky" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#0D1117"/>
      <stop offset=".55" stop-color="#0B2536"/>
      <stop offset="1" stop-color="#0B3A53"/>
    </linearGradient>
    <radialGradient id="neb1">
      <stop offset="0" stop-color="#61DAFB" stop-opacity=".22"/>
      <stop offset="1" stop-color="#61DAFB" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="neb2">
      <stop offset="0" stop-color="#8B5CF6" stop-opacity=".20"/>
      <stop offset="1" stop-color="#8B5CF6" stop-opacity="0"/>
    </radialGradient>
    <linearGradient id="ground" gradientUnits="userSpaceOnUse" x1="0" y1="285" x2="0" y2="360">
      <stop offset="0" stop-color="#1C7FA3"/>
      <stop offset="1" stop-color="#0B3A53"/>
    </linearGradient>
    <linearGradient id="planet" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#F7B267"/>
      <stop offset="1" stop-color="#E76F51"/>
    </linearGradient>
    <linearGradient id="visor" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#1F5673"/>
      <stop offset="1" stop-color="#0A1A26"/>
    </linearGradient>
    <linearGradient id="trail" gradientUnits="userSpaceOnUse" x1="0" y1="0" x2="90" y2="0">
      <stop offset="0" stop-color="#FFFFFF" stop-opacity="0"/>
      <stop offset="1" stop-color="#FFFFFF"/>
    </linearGradient>
    <clipPath id="frame">
      <rect width="1200" height="360" rx="24"/>
    </clipPath>
  </defs>

  <style>
    .float { animation: float 5s ease-in-out infinite; transform-origin: 160px 165px; }
    .wave  { animation: wave 1.6s ease-in-out infinite; transform-origin: 132px 190px; }
    .star  { animation: twinkle 2.6s ease-in-out infinite; }
    .blink { animation: twinkle 1.2s ease-in-out infinite; }
    .shoot { animation: shoot 7s ease-out infinite; }
    .d1 { animation-delay: .4s; }
    .d2 { animation-delay: .9s; }
    .d3 { animation-delay: 1.4s; }
    .d4 { animation-delay: 1.9s; }
    @keyframes float   { 0%, 100% { transform: translateY(6px) rotate(-3deg); } 50% { transform: translateY(-8px) rotate(3deg); } }
    @keyframes wave    { 0%, 100% { transform: rotate(-10deg); } 50% { transform: rotate(16deg); } }
    @keyframes twinkle { 0%, 100% { opacity: 1; } 50% { opacity: .25; } }
    @keyframes shoot   { 0% { transform: translateX(0); opacity: 0; } 3% { opacity: 1; } 14% { transform: translateX(190px); opacity: 0; } 100% { transform: translateX(190px); opacity: 0; } }
    @media (prefers-reduced-motion: reduce) { * { animation: none !important; } }
  </style>

  <g clip-path="url(#frame)">
    <!-- céu -->
    <rect width="1200" height="360" fill="url(#sky)"/>
    <ellipse cx="900" cy="110" rx="340" ry="210" fill="url(#neb1)"/>
    <ellipse cx="250" cy="230" rx="320" ry="190" fill="url(#neb2)"/>

    <!-- estrelas -->
    <g fill="#FFFFFF">
      <circle class="star"    cx="40"   cy="50"  r="1.8"/>
      <circle class="star d1" cx="15"   cy="120" r="1.4"/>
      <circle class="star d2" cx="95"   cy="160" r="2.2"/>
      <circle class="star d3" cx="130"  cy="30"  r="1.6"/>
      <circle class="star d4" cx="160"  cy="220" r="1.8"/>
      <circle class="star d1" cx="60"   cy="250" r="1.4"/>
      <circle class="star"    cx="240"  cy="150" r="2.4"/>
      <circle class="star d2" cx="270"  cy="250" r="1.6"/>
      <circle class="star d3" cx="300"  cy="60"  r="1.6"/>
      <circle class="star d4" cx="330"  cy="200" r="2"/>
      <circle class="star d1" cx="350"  cy="20"  r="1.4"/>
      <circle class="star"    cx="380"  cy="110" r="1.8"/>
      <circle class="star d2" cx="420"  cy="40"  r="2.2"/>
      <circle class="star d3" cx="450"  cy="240" r="1.6"/>
      <circle class="star d4" cx="480"  cy="180" r="1.4"/>
      <circle class="star d1" cx="505"  cy="70"  r="1.8"/>
      <circle class="star d2" cx="570"  cy="30"  r="1.4"/>
      <circle class="star"    cx="640"  cy="22"  r="2"/>
      <circle class="star d3" cx="700"  cy="60"  r="2.4"/>
      <circle class="star d4" cx="720"  cy="200" r="1.6"/>
      <circle class="star d1" cx="760"  cy="130" r="1.8"/>
      <circle class="star d2" cx="800"  cy="40"  r="1.4"/>
      <circle class="star"    cx="830"  cy="230" r="2"/>
      <circle class="star d3" cx="860"  cy="160" r="1.6"/>
      <circle class="star d4" cx="900"  cy="30"  r="2.2"/>
      <circle class="star d1" cx="930"  cy="210" r="1.4"/>
      <circle class="star d2" cx="1020" cy="250" r="1.6"/>
      <circle class="star"    cx="1040" cy="200" r="2.4"/>
      <circle class="star d3" cx="1080" cy="50"  r="1.8"/>
      <circle class="star d4" cx="1110" cy="140" r="1.6"/>
      <circle class="star d1" cx="1150" cy="90"  r="2"/>
      <circle class="star d2" cx="1170" cy="230" r="1.4"/>
      <circle class="star d3" cx="1190" cy="30"  r="1.6"/>
      <path class="star d2" transform="translate(430 150)"  d="M0 -9 L2 -2 L9 0 L2 2 L0 9 L-2 2 L-9 0 L-2 -2 Z"/>
      <path class="star d4" transform="translate(770 240)"  d="M0 -7 L1.6 -1.6 L7 0 L1.6 1.6 L0 7 L-1.6 1.6 L-7 0 L-1.6 -1.6 Z"/>
      <path class="star d1" transform="translate(1125 215)" d="M0 -8 L1.8 -1.8 L8 0 L1.8 1.8 L0 8 L-1.8 1.8 L-8 0 L-1.8 -1.8 Z"/>
      <path class="star d3" transform="translate(88 100)"   d="M0 -7 L1.6 -1.6 L7 0 L1.6 1.6 L0 7 L-1.6 1.6 L-7 0 L-1.6 -1.6 Z"/>
    </g>

    <!-- estrela cadente -->
    <g transform="translate(270 28) rotate(18)">
      <line class="shoot" x1="0" y1="0" x2="90" y2="0" stroke="url(#trail)" stroke-width="3" stroke-linecap="round"/>
    </g>

    <!-- lua -->
    <circle cx="190" cy="90" r="36" fill="#FFFFFF" fill-opacity=".06"/>
    <circle cx="190" cy="90" r="24" fill="#DCE6EE"/>
    <circle cx="182" cy="82" r="5" fill="#B8C4D0"/>
    <circle cx="198" cy="98" r="4" fill="#B8C4D0"/>
    <circle cx="200" cy="80" r="2.5" fill="#B8C4D0"/>

    <!-- planeta com anel -->
    <g transform="rotate(-18 980 104)">
      <ellipse cx="980" cy="104" rx="62" ry="13" fill="none" stroke="#FFE0B2" stroke-opacity=".9" stroke-width="5"/>
      <circle cx="980" cy="104" r="34" fill="url(#planet)"/>
      <circle cx="968" cy="92" r="11" fill="#FFFFFF" fill-opacity=".15"/>
      <path d="M918 104 A62 13 0 0 0 1042 104" fill="none" stroke="#FFE0B2" stroke-width="5" stroke-linecap="round"/>
    </g>

    <!-- horizonte -->
    <circle cx="600" cy="3285" r="3000" fill="url(#ground)"/>
    <circle cx="600" cy="3285" r="3000" fill="none" stroke="#61DAFB" stroke-opacity=".18" stroke-width="14"/>
    <circle cx="600" cy="3285" r="3000" fill="none" stroke="#61DAFB" stroke-opacity=".9" stroke-width="2"/>

    <!-- astronauta -->
    <g transform="translate(464 20) scale(.85)">
      <g class="float">
        <rect x="116" y="176" width="88" height="56" rx="16" fill="#9FB0C0"/>

        <g stroke="#E6EDF3" stroke-width="22" stroke-linecap="round">
          <line x1="148" y1="232" x2="141" y2="262"/>
          <line x1="172" y1="232" x2="179" y2="262"/>
        </g>
        <rect x="124" y="258" width="32" height="18" rx="9" fill="#61DAFB"/>
        <rect x="164" y="258" width="32" height="18" rx="9" fill="#61DAFB"/>

        <line x1="188" y1="192" x2="216" y2="212" stroke="#E6EDF3" stroke-width="20" stroke-linecap="round"/>
        <circle cx="219" cy="214" r="12" fill="#61DAFB"/>

        <g class="wave">
          <line x1="132" y1="190" x2="100" y2="162" stroke="#E6EDF3" stroke-width="20" stroke-linecap="round"/>
          <circle cx="97" cy="159" r="12" fill="#61DAFB"/>
        </g>

        <rect x="126" y="170" width="68" height="72" rx="26" fill="#FFFFFF"/>
        <rect x="144" y="198" width="32" height="20" rx="6" fill="#E6EDF3"/>
        <circle cx="154" cy="208" r="3.5" fill="#E0234E"/>
        <circle cx="166" cy="208" r="3.5" fill="#61DAFB"/>

        <line x1="160" y1="68" x2="160" y2="50" stroke="#9FB0C0" stroke-width="4" stroke-linecap="round"/>
        <circle class="blink" cx="160" cy="46" r="6" fill="#E0234E"/>

        <rect x="96" y="108" width="16" height="28" rx="8" fill="#9FB0C0"/>
        <rect x="208" y="108" width="16" height="28" rx="8" fill="#9FB0C0"/>
        <circle cx="160" cy="122" r="56" fill="#FFFFFF"/>
        <rect x="136" y="172" width="48" height="10" rx="5" fill="#61DAFB"/>

        <!-- visor só com o vidro -->
        <rect x="120" y="92" width="80" height="60" rx="28" fill="url(#visor)"/>
        <path d="M134 108 Q140 100 152 99" fill="none" stroke="#FFFFFF" stroke-opacity=".6" stroke-width="4" stroke-linecap="round"/>
        <path d="M128 123 Q128 117 130 113" fill="none" stroke="#FFFFFF" stroke-opacity=".4" stroke-width="3" stroke-linecap="round"/>
        <circle cx="184" cy="138" r="2" fill="#FFFFFF" fill-opacity=".5"/>
      </g>
    </g>
  </g>
</svg>
