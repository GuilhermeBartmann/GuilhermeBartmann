<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 320" width="320" height="320" role="img" aria-label="Astronauta flutuando no espaço">
  <defs>
    <linearGradient id="space" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#0D1117"/>
      <stop offset="1" stop-color="#0B3A53"/>
    </linearGradient>
    <linearGradient id="visor" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#1F5673"/>
      <stop offset="1" stop-color="#0A1A26"/>
    </linearGradient>
  </defs>

  <style>
    .float  { animation: float 5s ease-in-out infinite; transform-origin: 160px 165px; }
    .wave   { animation: wave 1.6s ease-in-out infinite; transform-origin: 132px 190px; }
    .orbit  { animation: orbit 14s linear infinite; transform-origin: 160px 160px; }
    .star   { animation: twinkle 2.4s ease-in-out infinite; }
    .blink  { animation: twinkle 1.2s ease-in-out infinite; }
    .d1 { animation-delay: .3s; }
    .d2 { animation-delay: .8s; }
    .d3 { animation-delay: 1.3s; }
    .d4 { animation-delay: 1.8s; }
    @keyframes float   { 0%, 100% { transform: translateY(6px) rotate(-3deg); } 50% { transform: translateY(-8px) rotate(3deg); } }
    @keyframes wave    { 0%, 100% { transform: rotate(-10deg); } 50% { transform: rotate(16deg); } }
    @keyframes orbit   { to { transform: rotate(360deg); } }
    @keyframes twinkle { 0%, 100% { opacity: 1; } 50% { opacity: .25; } }
    @media (prefers-reduced-motion: reduce) { * { animation: none !important; } }
  </style>

  <!-- espaço -->
  <circle cx="160" cy="160" r="140" fill="url(#space)"/>

  <!-- órbita com satélite -->
  <g class="orbit">
    <circle cx="160" cy="160" r="150" fill="none" stroke="#61DAFB" stroke-opacity=".45" stroke-width="2" stroke-linecap="round" stroke-dasharray="2 12"/>
    <circle cx="160" cy="10" r="5" fill="#61DAFB"/>
  </g>

  <!-- estrelas -->
  <g fill="#FFFFFF">
    <circle class="star"    cx="110" cy="60"  r="2.5"/>
    <circle class="star d1" cx="205" cy="48"  r="2"/>
    <circle class="star d2" cx="58"  cy="172" r="2"/>
    <circle class="star d3" cx="258" cy="146" r="2.5"/>
    <circle class="star d4" cx="242" cy="250" r="2"/>
    <circle class="star d1" cx="214" cy="272" r="2"/>
    <circle class="star d3" cx="44"  cy="140" r="1.8"/>
    <circle class="star d2" cx="276" cy="190" r="1.8"/>
    <path class="star d2" transform="translate(238 86)" d="M0 -9 L2 -2 L9 0 L2 2 L0 9 L-2 2 L-9 0 L-2 -2 Z"/>
    <path class="star d4" transform="translate(74 104)" d="M0 -7 L1.6 -1.6 L7 0 L1.6 1.6 L0 7 L-1.6 1.6 L-7 0 L-1.6 -1.6 Z"/>
  </g>

  <!-- planeta -->
  <circle cx="80" cy="238" r="13" fill="#F4A261"/>
  <ellipse cx="80" cy="238" rx="22" ry="5" fill="none" stroke="#FFE0B2" stroke-width="3" transform="rotate(-20 80 238)"/>

  <!-- astronauta -->
  <g class="float">
    <!-- mochila -->
    <rect x="116" y="176" width="88" height="56" rx="16" fill="#9FB0C0"/>

    <!-- pernas e botas -->
    <g stroke="#E6EDF3" stroke-width="22" stroke-linecap="round">
      <line x1="148" y1="232" x2="141" y2="262"/>
      <line x1="172" y1="232" x2="179" y2="262"/>
    </g>
    <rect x="124" y="258" width="32" height="18" rx="9" fill="#61DAFB"/>
    <rect x="164" y="258" width="32" height="18" rx="9" fill="#61DAFB"/>

    <!-- braço direito -->
    <line x1="188" y1="192" x2="216" y2="212" stroke="#E6EDF3" stroke-width="20" stroke-linecap="round"/>
    <circle cx="219" cy="214" r="12" fill="#61DAFB"/>

    <!-- braço esquerdo acenando -->
    <g class="wave">
      <line x1="132" y1="190" x2="100" y2="162" stroke="#E6EDF3" stroke-width="20" stroke-linecap="round"/>
      <circle cx="97" cy="159" r="12" fill="#61DAFB"/>
    </g>

    <!-- corpo -->
    <rect x="126" y="170" width="68" height="72" rx="26" fill="#FFFFFF"/>
    <rect x="144" y="198" width="32" height="20" rx="6" fill="#E6EDF3"/>
    <circle cx="154" cy="208" r="3.5" fill="#E0234E"/>
    <circle cx="166" cy="208" r="3.5" fill="#61DAFB"/>

    <!-- antena -->
    <line x1="160" y1="68" x2="160" y2="50" stroke="#9FB0C0" stroke-width="4" stroke-linecap="round"/>
    <circle class="blink" cx="160" cy="46" r="6" fill="#E0234E"/>

    <!-- capacete -->
    <rect x="96"  y="108" width="16" height="28" rx="8" fill="#9FB0C0"/>
    <rect x="208" y="108" width="16" height="28" rx="8" fill="#9FB0C0"/>
    <circle cx="160" cy="122" r="56" fill="#FFFFFF"/>
    <rect x="136" y="172" width="48" height="10" rx="5" fill="#61DAFB"/>

    <!-- visor e rosto -->
    <rect x="120" y="92" width="80" height="60" rx="28" fill="url(#visor)"/>
    <path d="M134 108 Q140 100 152 99" fill="none" stroke="#FFFFFF" stroke-opacity=".6" stroke-width="4" stroke-linecap="round"/>
    <circle cx="146" cy="122" r="5" fill="#FFFFFF"/>
    <circle cx="174" cy="122" r="5" fill="#FFFFFF"/>
    <circle cx="136" cy="133" r="4" fill="#FF8FA3" fill-opacity=".8"/>
    <circle cx="184" cy="133" r="4" fill="#FF8FA3" fill-opacity=".8"/>
    <path d="M151 134 Q160 142 169 134" fill="none" stroke="#FFFFFF" stroke-width="3" stroke-linecap="round"/>
  </g>
</svg>
