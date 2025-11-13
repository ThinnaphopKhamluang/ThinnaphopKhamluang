<!-- Cute animated penguin — paste this raw into your README.md -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 300 150" width="600" height="300" role="img" aria-label="Animated penguin">
  <!-- background (transparent) -->
  <!-- group for horizontal movement -->
  <g id="moveGroup">
    <!-- group for vertical bobbing -->
    <g id="bobGroup">
      <!-- body -->
      <ellipse cx="150" cy="90" rx="42" ry="56" fill="#0b2233"/>
      <!-- belly -->
      <ellipse cx="150" cy="96" rx="28" ry="40" fill="#fff"/>
      <!-- head -->
      <circle cx="150" cy="46" r="28" fill="#0b2233"/>
      <!-- face white -->
      <ellipse cx="150" cy="52" rx="16" ry="12" fill="#fff"/>
      <!-- eyes -->
      <circle cx="142" cy="50" r="3.5" fill="#000"/>
      <circle cx="158" cy="50" r="3.5" fill="#000"/>
      <!-- beak -->
      <path d="M150 58 L142 66 Q150 63 158 66 Z" fill="#ffb03b"/>
      <!-- left wing -->
      <path d="M110 90 Q116 78 126 92 Q118 100 110 98 Z" fill="#0b2233"/>
      <!-- right wing -->
      <path d="M190 90 Q184 78 174 92 Q182 100 190 98 Z" fill="#0b2233"/>
      <!-- left foot -->
      <path d="M136 137 Q142 130 148 137 Q142 142 136 137 Z" fill="#ffb03b"/>
      <!-- right foot -->
      <path d="M152 137 Q158 130 164 137 Q158 142 152 137 Z" fill="#ffb03b"/>
      <!-- small scarf -->
      <rect x="132" y="70" width="36" height="8" rx="3" fill="#ff6b6b"/>
      <path d="M166 74 Q178 80 172 86 L170 82 Q176 78 166 74 Z" fill="#ff6b6b" opacity="0.9"/>
    </g>
    <!-- add a subtle shadow -->
    <ellipse cx="150" cy="145" rx="36" ry="8" fill="#000" opacity="0.12"/>
  </g>

  <!-- Horizontal movement: left-right -->
  <animateTransform
    xlink:href="#moveGroup"
    attributeName="transform"
    type="translate"
    values="-30 0; 30 0; -30 0"
