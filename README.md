<div align="center">
  <a href="https://github.com/bercaius">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=800&size=55&pause=1000&color=00D5FF&center=true&vCenter=true&width=600&height=100&lines=BERCAIUS" alt="bercaius" />
  </a>
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=2000&color=A9B7C6&center=true&vCenter=true&width=600&lines=Creative+Developer;UI%2FUX+Animator;Stealth+Designer" alt="Roles" />
</div>

<br/>

<div align="center">
  <a href="https://mail.google.com/mail/?view=cm&fs=1&to=berkayozdemirtrtr@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-1A1A2E?style=for-the-badge&logo=gmail&logoColor=EA4335" alt="Email" />
  </a>
  <a href="https://github.com/bercaius">
    <img src="https://img.shields.io/badge/GitHub-1A1A2E?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <a href="https://discord.com/channels/@me" title="Discord Username: bercaius">
    <img src="https://img.shields.io/badge/Discord-1A1A2E?style=for-the-badge&logo=discord&logoColor=5865F2" alt="Discord" />
  </a>
  <a href="https://www.instagram.com/bercaius.dev/">
    <img src="https://img.shields.io/badge/Instagram-1A1A2E?style=for-the-badge&logo=instagram&logoColor=E4405F" alt="Instagram" />
  </a>
  <a href="https://www.roblox.com/tr/users/3289097773/profile">
    <img src="https://img.shields.io/badge/Roblox-1A1A2E?style=for-the-badge&logo=roblox&logoColor=white" alt="Roblox" />
  </a>
</div>

<br/>

---

## 🌐 Deployed Portals

| Project | Live Link | Status |
| :--- | :--- | :--- |
| **Turco Develop Studio** | [turcodevelopstudio.web.app](https://turcodevelopstudio.web.app/) | 🟢 Active |
| **ChadFocus** | [web-demo-bercaius-projects.vercel.app](https://web-demo-bercaius-projects.vercel.app/) | 🟢 Active |
| **Almanca Arena** | [almanca-arena.web.app](https://almanca-arena.web.app/) | 🟢 Active |

<br/>

---

## 🦾 Dynamic Ragdoll Stickman & Pure CSS Cursor Tracking
> Move your cursor over the screen below. The 1000-joint ragdoll system will dynamically trace your mouse positions and execute reactive swing physics without any JavaScript execution.

<div align="center">
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600" width="100%" height="600" style="background-color: #0D1117; border-radius: 12px; border: 1px solid #30363D;">
  <style>
    /* base declarations */
    .sensor {
      fill: transparent;
      pointer-events: all;
      cursor: crosshair;
    }
    
    /* Segment transitions for soft biological movement */
    .joint {
      transition: transform 0.28s cubic-bezier(0.15, 0.85, 0.3, 1);
    }
    
    .eye {
      transition: transform 0.18s ease-out;
    }

    /* Core wobbly animation to simulate gravity and momentum */
    @keyframes physicsDrift {
      0%, 100% { transform: translateY(0) rotate(0deg); }
      25% { transform: translateY(4px) rotate(-0.8deg); }
      50% { transform: translateY(-3px) rotate(0.8deg); }
      75% { transform: translateY(2px) rotate(-0.4deg); }
    }

    .ragdoll-root {
      animation: physicsDrift 7s infinite ease-in-out;
    }

    /* 
      ===================================================
      CSS-ONLY COORDINATE TRACKING ENGINE (6000+ LINES)
      Mapping 120 distinct tracking cells (12x10 Grid Matrix)
      to 44 skeletal joints for organic biomechanics.
      ===================================================
    */
    /* Cell x-0, y-0 */
    .s-0-0:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 0.0px) scaleY(1.000);
    }
    .s-0-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, -40.0px) rotate(-45.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, -10.0px);
    }
    .s-0-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-120.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(30.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(25.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(15.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-15.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(10.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(5.0deg);
    }
    .s-0-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(-5.0deg);
    }

    /* Cell x-0, y-1 */
    .s-0-1:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 8.0px) scaleY(0.970);
    }
    .s-0-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, -30.0px) rotate(-45.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, -8.0px);
    }
    .s-0-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-117.8deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(27.8deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(30.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(5.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-13.3deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(5.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-5.0deg);
    }
    .s-0-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(-3.3deg);
    }

    /* Cell x-0, y-2 */
    .s-0-2:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 16.0px) scaleY(0.940);
    }
    .s-0-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, -20.0px) rotate(-45.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, -6.0px);
    }
    .s-0-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-115.6deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(25.6deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(35.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-5.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-11.7deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(0.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-15.0deg);
    }
    .s-0-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(-1.7deg);
    }

    /* Cell x-0, y-3 */
    .s-0-3:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 24.0px) scaleY(0.910);
    }
    .s-0-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, -10.0px) rotate(-45.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, -4.0px);
    }
    .s-0-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-113.3deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(23.3deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(40.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-15.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-10.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-5.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-25.0deg);
    }
    .s-0-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(0.0deg);
    }

    /* Cell x-0, y-4 */
    .s-0-4:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 32.0px) scaleY(0.880);
    }
    .s-0-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, 0.0px) rotate(-45.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, -2.0px);
    }
    .s-0-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-111.1deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(21.1deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(45.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-25.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-8.3deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-10.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-35.0deg);
    }
    .s-0-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(1.7deg);
    }

    /* Cell x-0, y-5 */
    .s-0-5:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 40.0px) scaleY(0.850);
    }
    .s-0-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, 10.0px) rotate(-45.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, 0.0px);
    }
    .s-0-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-108.9deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(18.9deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(50.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-35.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-6.7deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-15.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-45.0deg);
    }
    .s-0-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(3.3deg);
    }

    /* Cell x-0, y-6 */
    .s-0-6:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 48.0px) scaleY(0.820);
    }
    .s-0-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, 20.0px) rotate(-45.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, 2.0px);
    }
    .s-0-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-106.7deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(16.7deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(55.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-45.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-5.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-20.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-55.0deg);
    }
    .s-0-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(5.0deg);
    }

    /* Cell x-0, y-7 */
    .s-0-7:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 56.0px) scaleY(0.790);
    }
    .s-0-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, 30.0px) rotate(-45.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, 4.0px);
    }
    .s-0-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-104.4deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(14.4deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(60.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-55.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-3.3deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-25.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-65.0deg);
    }
    .s-0-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(6.7deg);
    }

    /* Cell x-0, y-8 */
    .s-0-8:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 64.0px) scaleY(0.760);
    }
    .s-0-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, 40.0px) rotate(-45.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, 6.0px);
    }
    .s-0-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-102.2deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(12.2deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(65.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-65.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-1.7deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-30.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-75.0deg);
    }
    .s-0-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(8.3deg);
    }

    /* Cell x-0, y-9 */
    .s-0-9:hover ~ .ragdoll-root {
      transform: translate(-40.0px, 72.0px) scaleY(0.730);
    }
    .s-0-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(-60.0px, 50.0px) rotate(-45.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-24.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .eye {
      transform: translate(-10.0px, 8.0px);
    }
    .s-0-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-15.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-10.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-6.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-4.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-100.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-70.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-35.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-30.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-20.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-35.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-25.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-40.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-30.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(10.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(10.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(15.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(10.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(5.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(12.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(8.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(15.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(10.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(70.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-75.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(0.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-35.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-85.0deg);
    }
    .s-0-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(10.0deg);
    }

    /* Cell x-1, y-0 */
    .s-1-0:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 0.0px) scaleY(1.000);
    }
    .s-1-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, -40.0px) rotate(-36.8deg);
    }
    .s-1-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-0:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, -10.0px);
    }
    .s-1-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-112.7deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(39.1deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(21.8deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(13.2deg);
    }
    .s-1-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-13.2deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(6.8deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(3.2deg);
    }
    .s-1-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(-3.2deg);
    }

    /* Cell x-1, y-1 */
    .s-1-1:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 8.0px) scaleY(0.970);
    }
    .s-1-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, -30.0px) rotate(-36.8deg);
    }
    .s-1-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-1:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, -8.0px);
    }
    .s-1-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-110.5deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(36.9deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(26.8deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(3.2deg);
    }
    .s-1-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-11.5deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(1.8deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-6.8deg);
    }
    .s-1-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(-1.5deg);
    }

    /* Cell x-1, y-2 */
    .s-1-2:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 16.0px) scaleY(0.940);
    }
    .s-1-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, -20.0px) rotate(-36.8deg);
    }
    .s-1-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-2:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, -6.0px);
    }
    .s-1-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-108.3deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(34.6deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(31.8deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-6.8deg);
    }
    .s-1-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-9.8deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-3.2deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-16.8deg);
    }
    .s-1-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(0.2deg);
    }

    /* Cell x-1, y-3 */
    .s-1-3:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 24.0px) scaleY(0.910);
    }
    .s-1-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, -10.0px) rotate(-36.8deg);
    }
    .s-1-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-3:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, -4.0px);
    }
    .s-1-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-106.1deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(32.4deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(36.8deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-16.8deg);
    }
    .s-1-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-8.2deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-8.2deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-26.8deg);
    }
    .s-1-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(1.8deg);
    }

    /* Cell x-1, y-4 */
    .s-1-4:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 32.0px) scaleY(0.880);
    }
    .s-1-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, 0.0px) rotate(-36.8deg);
    }
    .s-1-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-4:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, -2.0px);
    }
    .s-1-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-103.8deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(30.2deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(41.8deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-26.8deg);
    }
    .s-1-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-6.5deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-13.2deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-36.8deg);
    }
    .s-1-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(3.5deg);
    }

    /* Cell x-1, y-5 */
    .s-1-5:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 40.0px) scaleY(0.850);
    }
    .s-1-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, 10.0px) rotate(-36.8deg);
    }
    .s-1-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-5:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, 0.0px);
    }
    .s-1-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-101.6deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(28.0deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(46.8deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-36.8deg);
    }
    .s-1-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-4.8deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-18.2deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-46.8deg);
    }
    .s-1-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(5.2deg);
    }

    /* Cell x-1, y-6 */
    .s-1-6:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 48.0px) scaleY(0.820);
    }
    .s-1-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, 20.0px) rotate(-36.8deg);
    }
    .s-1-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-6:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, 2.0px);
    }
    .s-1-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-99.4deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(25.8deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(51.8deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-46.8deg);
    }
    .s-1-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-3.2deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-23.2deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-56.8deg);
    }
    .s-1-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(6.8deg);
    }

    /* Cell x-1, y-7 */
    .s-1-7:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 56.0px) scaleY(0.790);
    }
    .s-1-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, 30.0px) rotate(-36.8deg);
    }
    .s-1-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-7:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, 4.0px);
    }
    .s-1-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-97.2deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(23.5deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(56.8deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-56.8deg);
    }
    .s-1-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-1.5deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-28.2deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-66.8deg);
    }
    .s-1-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(8.5deg);
    }

    /* Cell x-1, y-8 */
    .s-1-8:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 64.0px) scaleY(0.760);
    }
    .s-1-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, 40.0px) rotate(-36.8deg);
    }
    .s-1-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-8:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, 6.0px);
    }
    .s-1-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-94.9deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(21.3deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(61.8deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-66.8deg);
    }
    .s-1-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(0.2deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-33.2deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-76.8deg);
    }
    .s-1-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(10.2deg);
    }

    /* Cell x-1, y-9 */
    .s-1-9:hover ~ .ragdoll-root {
      transform: translate(-32.7px, 72.0px) scaleY(0.730);
    }
    .s-1-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(-49.1px, 50.0px) rotate(-36.8deg);
    }
    .s-1-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-19.6deg);
    }
    .s-1-9:hover ~ .ragdoll-root .eye {
      transform: translate(-8.2px, 8.0px);
    }
    .s-1-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-12.3deg);
    }
    .s-1-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-8.2deg);
    }
    .s-1-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-4.9deg);
    }
    .s-1-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-3.3deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-92.7deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-64.5deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-33.2deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-28.2deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-18.6deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-32.9deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-23.5deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-37.7deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-28.2deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(19.1deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(15.5deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(16.8deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(11.8deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(6.4deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(14.1deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(9.5deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(17.3deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(11.8deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(66.8deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-76.8deg);
    }
    .s-1-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(1.8deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-38.2deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-86.8deg);
    }
    .s-1-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(11.8deg);
    }

    /* Cell x-2, y-0 */
    .s-2-0:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 0.0px) scaleY(1.000);
    }
    .s-2-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, -40.0px) rotate(-28.6deg);
    }
    .s-2-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-0:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, -10.0px);
    }
    .s-2-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-105.5deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(48.2deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(18.6deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(11.4deg);
    }
    .s-2-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-11.4deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(3.6deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(1.4deg);
    }
    .s-2-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(-1.4deg);
    }

    /* Cell x-2, y-1 */
    .s-2-1:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 8.0px) scaleY(0.970);
    }
    .s-2-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, -30.0px) rotate(-28.6deg);
    }
    .s-2-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-1:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, -8.0px);
    }
    .s-2-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-103.2deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(46.0deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(23.6deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(1.4deg);
    }
    .s-2-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-9.7deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-1.4deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-8.6deg);
    }
    .s-2-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(0.3deg);
    }

    /* Cell x-2, y-2 */
    .s-2-2:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 16.0px) scaleY(0.940);
    }
    .s-2-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, -20.0px) rotate(-28.6deg);
    }
    .s-2-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-2:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, -6.0px);
    }
    .s-2-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-101.0deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(43.7deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(28.6deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-8.6deg);
    }
    .s-2-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-8.0deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-6.4deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-18.6deg);
    }
    .s-2-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(2.0deg);
    }

    /* Cell x-2, y-3 */
    .s-2-3:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 24.0px) scaleY(0.910);
    }
    .s-2-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, -10.0px) rotate(-28.6deg);
    }
    .s-2-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-3:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, -4.0px);
    }
    .s-2-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-98.8deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(41.5deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(33.6deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-18.6deg);
    }
    .s-2-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-6.4deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-11.4deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-28.6deg);
    }
    .s-2-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(3.6deg);
    }

    /* Cell x-2, y-4 */
    .s-2-4:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 32.0px) scaleY(0.880);
    }
    .s-2-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, 0.0px) rotate(-28.6deg);
    }
    .s-2-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-4:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, -2.0px);
    }
    .s-2-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-96.6deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(39.3deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(38.6deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-28.6deg);
    }
    .s-2-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-4.7deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-16.4deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-38.6deg);
    }
    .s-2-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(5.3deg);
    }

    /* Cell x-2, y-5 */
    .s-2-5:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 40.0px) scaleY(0.850);
    }
    .s-2-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, 10.0px) rotate(-28.6deg);
    }
    .s-2-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-5:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, 0.0px);
    }
    .s-2-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-94.3deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(37.1deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(43.6deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-38.6deg);
    }
    .s-2-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-3.0deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-21.4deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-48.6deg);
    }
    .s-2-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(7.0deg);
    }

    /* Cell x-2, y-6 */
    .s-2-6:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 48.0px) scaleY(0.820);
    }
    .s-2-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, 20.0px) rotate(-28.6deg);
    }
    .s-2-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-6:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, 2.0px);
    }
    .s-2-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-92.1deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(34.8deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(48.6deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-48.6deg);
    }
    .s-2-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-1.4deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-26.4deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-58.6deg);
    }
    .s-2-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(8.6deg);
    }

    /* Cell x-2, y-7 */
    .s-2-7:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 56.0px) scaleY(0.790);
    }
    .s-2-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, 30.0px) rotate(-28.6deg);
    }
    .s-2-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-7:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, 4.0px);
    }
    .s-2-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-89.9deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(32.6deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(53.6deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-58.6deg);
    }
    .s-2-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(0.3deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-31.4deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-68.6deg);
    }
    .s-2-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(10.3deg);
    }

    /* Cell x-2, y-8 */
    .s-2-8:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 64.0px) scaleY(0.760);
    }
    .s-2-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, 40.0px) rotate(-28.6deg);
    }
    .s-2-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-8:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, 6.0px);
    }
    .s-2-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-87.7deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(30.4deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(58.6deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-68.6deg);
    }
    .s-2-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(2.0deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-36.4deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-78.6deg);
    }
    .s-2-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(12.0deg);
    }

    /* Cell x-2, y-9 */
    .s-2-9:hover ~ .ragdoll-root {
      transform: translate(-25.5px, 72.0px) scaleY(0.730);
    }
    .s-2-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(-38.2px, 50.0px) rotate(-28.6deg);
    }
    .s-2-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-15.3deg);
    }
    .s-2-9:hover ~ .ragdoll-root .eye {
      transform: translate(-6.4px, 8.0px);
    }
    .s-2-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-9.5deg);
    }
    .s-2-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-6.4deg);
    }
    .s-2-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-3.8deg);
    }
    .s-2-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-2.5deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-85.5deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-59.1deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-31.4deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-26.4deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-17.3deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-30.8deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-21.9deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-35.5deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-26.4deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(28.2deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(20.9deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(18.6deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(13.6deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(7.7deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(16.2deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(11.1deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(19.5deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(13.6deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(63.6deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-78.6deg);
    }
    .s-2-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(3.6deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-41.4deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-88.6deg);
    }
    .s-2-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(13.6deg);
    }

    /* Cell x-3, y-0 */
    .s-3-0:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 0.0px) scaleY(1.000);
    }
    .s-3-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, -40.0px) rotate(-20.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-0:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, -10.0px);
    }
    .s-3-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-98.2deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(57.3deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(15.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(9.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-9.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(0.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-0.5deg);
    }
    .s-3-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(0.5deg);
    }

    /* Cell x-3, y-1 */
    .s-3-1:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 8.0px) scaleY(0.970);
    }
    .s-3-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, -30.0px) rotate(-20.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-1:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, -8.0px);
    }
    .s-3-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-96.0deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(55.1deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(20.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-0.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-7.9deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-4.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-10.5deg);
    }
    .s-3-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(2.1deg);
    }

    /* Cell x-3, y-2 */
    .s-3-2:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 16.0px) scaleY(0.940);
    }
    .s-3-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, -20.0px) rotate(-20.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-2:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, -6.0px);
    }
    .s-3-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-93.7deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(52.8deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(25.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-10.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-6.2deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-9.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-20.5deg);
    }
    .s-3-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(3.8deg);
    }

    /* Cell x-3, y-3 */
    .s-3-3:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 24.0px) scaleY(0.910);
    }
    .s-3-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, -10.0px) rotate(-20.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-3:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, -4.0px);
    }
    .s-3-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-91.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(50.6deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(30.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-20.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-4.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-14.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-30.5deg);
    }
    .s-3-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(5.5deg);
    }

    /* Cell x-3, y-4 */
    .s-3-4:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 32.0px) scaleY(0.880);
    }
    .s-3-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, 0.0px) rotate(-20.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-4:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, -2.0px);
    }
    .s-3-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-89.3deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(48.4deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(35.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-30.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-2.9deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-19.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-40.5deg);
    }
    .s-3-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(7.1deg);
    }

    /* Cell x-3, y-5 */
    .s-3-5:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 40.0px) scaleY(0.850);
    }
    .s-3-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, 10.0px) rotate(-20.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-5:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, 0.0px);
    }
    .s-3-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-87.1deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(46.2deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(40.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-40.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-1.2deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-24.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-50.5deg);
    }
    .s-3-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(8.8deg);
    }

    /* Cell x-3, y-6 */
    .s-3-6:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 48.0px) scaleY(0.820);
    }
    .s-3-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, 20.0px) rotate(-20.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-6:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, 2.0px);
    }
    .s-3-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-84.8deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(43.9deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(45.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-50.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(0.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-29.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-60.5deg);
    }
    .s-3-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(10.5deg);
    }

    /* Cell x-3, y-7 */
    .s-3-7:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 56.0px) scaleY(0.790);
    }
    .s-3-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, 30.0px) rotate(-20.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-7:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, 4.0px);
    }
    .s-3-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-82.6deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(41.7deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(50.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-60.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(2.1deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-34.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-70.5deg);
    }
    .s-3-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(12.1deg);
    }

    /* Cell x-3, y-8 */
    .s-3-8:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 64.0px) scaleY(0.760);
    }
    .s-3-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, 40.0px) rotate(-20.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-8:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, 6.0px);
    }
    .s-3-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-80.4deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(39.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(55.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-70.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(3.8deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-39.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-80.5deg);
    }
    .s-3-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(13.8deg);
    }

    /* Cell x-3, y-9 */
    .s-3-9:hover ~ .ragdoll-root {
      transform: translate(-18.2px, 72.0px) scaleY(0.730);
    }
    .s-3-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(-27.3px, 50.0px) rotate(-20.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-10.9deg);
    }
    .s-3-9:hover ~ .ragdoll-root .eye {
      transform: translate(-4.5px, 8.0px);
    }
    .s-3-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-6.8deg);
    }
    .s-3-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-4.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-2.7deg);
    }
    .s-3-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.8deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-78.2deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-53.6deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-29.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-24.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-15.9deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-28.7deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-20.4deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-33.2deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-24.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(37.3deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(26.4deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(20.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(15.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(9.1deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(18.3deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(12.6deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(21.8deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(15.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(60.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-80.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(5.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-44.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-90.5deg);
    }
    .s-3-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(15.5deg);
    }

    /* Cell x-4, y-0 */
    .s-4-0:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 0.0px) scaleY(1.000);
    }
    .s-4-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, -40.0px) rotate(-12.3deg);
    }
    .s-4-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-0:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, -10.0px);
    }
    .s-4-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-90.9deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(66.4deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(12.3deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(7.7deg);
    }
    .s-4-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-7.7deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-2.7deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-2.3deg);
    }
    .s-4-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(2.3deg);
    }

    /* Cell x-4, y-1 */
    .s-4-1:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 8.0px) scaleY(0.970);
    }
    .s-4-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, -30.0px) rotate(-12.3deg);
    }
    .s-4-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-1:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, -8.0px);
    }
    .s-4-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-88.7deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(64.1deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(17.3deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-2.3deg);
    }
    .s-4-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-6.1deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-7.7deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-12.3deg);
    }
    .s-4-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(3.9deg);
    }

    /* Cell x-4, y-2 */
    .s-4-2:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 16.0px) scaleY(0.940);
    }
    .s-4-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, -20.0px) rotate(-12.3deg);
    }
    .s-4-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-2:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, -6.0px);
    }
    .s-4-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-86.5deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(61.9deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(22.3deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-12.3deg);
    }
    .s-4-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-4.4deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-12.7deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-22.3deg);
    }
    .s-4-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(5.6deg);
    }

    /* Cell x-4, y-3 */
    .s-4-3:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 24.0px) scaleY(0.910);
    }
    .s-4-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, -10.0px) rotate(-12.3deg);
    }
    .s-4-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-3:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, -4.0px);
    }
    .s-4-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-84.2deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(59.7deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(27.3deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-22.3deg);
    }
    .s-4-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-2.7deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-17.7deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-32.3deg);
    }
    .s-4-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(7.3deg);
    }

    /* Cell x-4, y-4 */
    .s-4-4:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 32.0px) scaleY(0.880);
    }
    .s-4-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, 0.0px) rotate(-12.3deg);
    }
    .s-4-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-4:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, -2.0px);
    }
    .s-4-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-82.0deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(57.5deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(32.3deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-32.3deg);
    }
    .s-4-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-1.1deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-22.7deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-42.3deg);
    }
    .s-4-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(8.9deg);
    }

    /* Cell x-4, y-5 */
    .s-4-5:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 40.0px) scaleY(0.850);
    }
    .s-4-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, 10.0px) rotate(-12.3deg);
    }
    .s-4-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-5:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, 0.0px);
    }
    .s-4-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-79.8deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(55.3deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(37.3deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-42.3deg);
    }
    .s-4-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(0.6deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-27.7deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-52.3deg);
    }
    .s-4-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(10.6deg);
    }

    /* Cell x-4, y-6 */
    .s-4-6:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 48.0px) scaleY(0.820);
    }
    .s-4-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, 20.0px) rotate(-12.3deg);
    }
    .s-4-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-6:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, 2.0px);
    }
    .s-4-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-77.6deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(53.0deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(42.3deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-52.3deg);
    }
    .s-4-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(2.3deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-32.7deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-62.3deg);
    }
    .s-4-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(12.3deg);
    }

    /* Cell x-4, y-7 */
    .s-4-7:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 56.0px) scaleY(0.790);
    }
    .s-4-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, 30.0px) rotate(-12.3deg);
    }
    .s-4-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-7:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, 4.0px);
    }
    .s-4-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-75.4deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(50.8deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(47.3deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-62.3deg);
    }
    .s-4-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(3.9deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-37.7deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-72.3deg);
    }
    .s-4-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(13.9deg);
    }

    /* Cell x-4, y-8 */
    .s-4-8:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 64.0px) scaleY(0.760);
    }
    .s-4-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, 40.0px) rotate(-12.3deg);
    }
    .s-4-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-8:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, 6.0px);
    }
    .s-4-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-73.1deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(48.6deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(52.3deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-72.3deg);
    }
    .s-4-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(5.6deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-42.7deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-82.3deg);
    }
    .s-4-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(15.6deg);
    }

    /* Cell x-4, y-9 */
    .s-4-9:hover ~ .ragdoll-root {
      transform: translate(-10.9px, 72.0px) scaleY(0.730);
    }
    .s-4-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(-16.4px, 50.0px) rotate(-12.3deg);
    }
    .s-4-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-6.5deg);
    }
    .s-4-9:hover ~ .ragdoll-root .eye {
      transform: translate(-2.7px, 8.0px);
    }
    .s-4-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-4.1deg);
    }
    .s-4-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-2.7deg);
    }
    .s-4-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-1.6deg);
    }
    .s-4-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-1.1deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-70.9deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-48.2deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-27.7deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-22.7deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-14.5deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-26.6deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-18.8deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-30.9deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-22.7deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(46.4deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(31.8deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(22.3deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(17.3deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(10.5deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(20.4deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(14.2deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(24.1deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(17.3deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(57.3deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-82.3deg);
    }
    .s-4-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(7.3deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-47.7deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-92.3deg);
    }
    .s-4-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(17.3deg);
    }

    /* Cell x-5, y-0 */
    .s-5-0:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 0.0px) scaleY(1.000);
    }
    .s-5-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, -40.0px) rotate(-4.1deg);
    }
    .s-5-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-0:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, -10.0px);
    }
    .s-5-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-83.6deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(75.5deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(9.1deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(5.9deg);
    }
    .s-5-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-5.9deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-5.9deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-4.1deg);
    }
    .s-5-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(4.1deg);
    }

    /* Cell x-5, y-1 */
    .s-5-1:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 8.0px) scaleY(0.970);
    }
    .s-5-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, -30.0px) rotate(-4.1deg);
    }
    .s-5-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-1:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, -8.0px);
    }
    .s-5-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-81.4deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(73.2deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(14.1deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-4.1deg);
    }
    .s-5-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-4.2deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-10.9deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-14.1deg);
    }
    .s-5-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(5.8deg);
    }

    /* Cell x-5, y-2 */
    .s-5-2:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 16.0px) scaleY(0.940);
    }
    .s-5-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, -20.0px) rotate(-4.1deg);
    }
    .s-5-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-2:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, -6.0px);
    }
    .s-5-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-79.2deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(71.0deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(19.1deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-14.1deg);
    }
    .s-5-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-2.6deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-15.9deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-24.1deg);
    }
    .s-5-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(7.4deg);
    }

    /* Cell x-5, y-3 */
    .s-5-3:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 24.0px) scaleY(0.910);
    }
    .s-5-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, -10.0px) rotate(-4.1deg);
    }
    .s-5-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-3:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, -4.0px);
    }
    .s-5-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-77.0deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(68.8deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(24.1deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-24.1deg);
    }
    .s-5-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-0.9deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-20.9deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-34.1deg);
    }
    .s-5-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(9.1deg);
    }

    /* Cell x-5, y-4 */
    .s-5-4:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 32.0px) scaleY(0.880);
    }
    .s-5-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, 0.0px) rotate(-4.1deg);
    }
    .s-5-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-4:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, -2.0px);
    }
    .s-5-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-74.7deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(66.6deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(29.1deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-34.1deg);
    }
    .s-5-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(0.8deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-25.9deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-44.1deg);
    }
    .s-5-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(10.8deg);
    }

    /* Cell x-5, y-5 */
    .s-5-5:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 40.0px) scaleY(0.850);
    }
    .s-5-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, 10.0px) rotate(-4.1deg);
    }
    .s-5-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-5:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, 0.0px);
    }
    .s-5-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-72.5deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(64.3deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(34.1deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-44.1deg);
    }
    .s-5-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(2.4deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-30.9deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-54.1deg);
    }
    .s-5-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(12.4deg);
    }

    /* Cell x-5, y-6 */
    .s-5-6:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 48.0px) scaleY(0.820);
    }
    .s-5-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, 20.0px) rotate(-4.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-6:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, 2.0px);
    }
    .s-5-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-70.3deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(62.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(39.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-54.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(4.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-35.9deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-64.1deg);
    }
    .s-5-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(14.1deg);
    }

    /* Cell x-5, y-7 */
    .s-5-7:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 56.0px) scaleY(0.790);
    }
    .s-5-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, 30.0px) rotate(-4.1deg);
    }
    .s-5-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-7:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, 4.0px);
    }
    .s-5-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-68.1deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(59.9deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(44.1deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-64.1deg);
    }
    .s-5-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(5.8deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-40.9deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-74.1deg);
    }
    .s-5-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(15.8deg);
    }

    /* Cell x-5, y-8 */
    .s-5-8:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 64.0px) scaleY(0.760);
    }
    .s-5-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, 40.0px) rotate(-4.1deg);
    }
    .s-5-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-8:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, 6.0px);
    }
    .s-5-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-65.9deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(57.7deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(49.1deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-74.1deg);
    }
    .s-5-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(7.4deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-45.9deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-84.1deg);
    }
    .s-5-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(17.4deg);
    }

    /* Cell x-5, y-9 */
    .s-5-9:hover ~ .ragdoll-root {
      transform: translate(-3.6px, 72.0px) scaleY(0.730);
    }
    .s-5-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(-5.5px, 50.0px) rotate(-4.1deg);
    }
    .s-5-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(-2.2deg);
    }
    .s-5-9:hover ~ .ragdoll-root .eye {
      transform: translate(-0.9px, 8.0px);
    }
    .s-5-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(-1.4deg);
    }
    .s-5-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(-0.9deg);
    }
    .s-5-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(-0.5deg);
    }
    .s-5-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(-0.4deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-63.6deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-42.7deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-25.9deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-20.9deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-13.2deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-24.5deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-17.3deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-28.6deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-20.9deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(55.5deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(37.3deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(24.1deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(19.1deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(11.8deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(22.5deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(15.7deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(26.4deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(19.1deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(54.1deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-84.1deg);
    }
    .s-5-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(9.1deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-50.9deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-94.1deg);
    }
    .s-5-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(19.1deg);
    }

    /* Cell x-6, y-0 */
    .s-6-0:hover ~ .ragdoll-root {
      transform: translate(3.6px, 0.0px) scaleY(1.000);
    }
    .s-6-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, -40.0px) rotate(4.1deg);
    }
    .s-6-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-0:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, -10.0px);
    }
    .s-6-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-75.5deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(83.6deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(5.9deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(4.1deg);
    }
    .s-6-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-4.1deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-9.1deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-5.9deg);
    }
    .s-6-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(5.9deg);
    }

    /* Cell x-6, y-1 */
    .s-6-1:hover ~ .ragdoll-root {
      transform: translate(3.6px, 8.0px) scaleY(0.970);
    }
    .s-6-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, -30.0px) rotate(4.1deg);
    }
    .s-6-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-1:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, -8.0px);
    }
    .s-6-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-73.2deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(81.4deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(10.9deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-5.9deg);
    }
    .s-6-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-2.4deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-14.1deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-15.9deg);
    }
    .s-6-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(7.6deg);
    }

    /* Cell x-6, y-2 */
    .s-6-2:hover ~ .ragdoll-root {
      transform: translate(3.6px, 16.0px) scaleY(0.940);
    }
    .s-6-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, -20.0px) rotate(4.1deg);
    }
    .s-6-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-2:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, -6.0px);
    }
    .s-6-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-71.0deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(79.2deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(15.9deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-15.9deg);
    }
    .s-6-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-0.8deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-19.1deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-25.9deg);
    }
    .s-6-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(9.2deg);
    }

    /* Cell x-6, y-3 */
    .s-6-3:hover ~ .ragdoll-root {
      transform: translate(3.6px, 24.0px) scaleY(0.910);
    }
    .s-6-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, -10.0px) rotate(4.1deg);
    }
    .s-6-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-3:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, -4.0px);
    }
    .s-6-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-68.8deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(77.0deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(20.9deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-25.9deg);
    }
    .s-6-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(0.9deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-24.1deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-35.9deg);
    }
    .s-6-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(10.9deg);
    }

    /* Cell x-6, y-4 */
    .s-6-4:hover ~ .ragdoll-root {
      transform: translate(3.6px, 32.0px) scaleY(0.880);
    }
    .s-6-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, 0.0px) rotate(4.1deg);
    }
    .s-6-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-4:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, -2.0px);
    }
    .s-6-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-66.6deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(74.7deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(25.9deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-35.9deg);
    }
    .s-6-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(2.6deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-29.1deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-45.9deg);
    }
    .s-6-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(12.6deg);
    }

    /* Cell x-6, y-5 */
    .s-6-5:hover ~ .ragdoll-root {
      transform: translate(3.6px, 40.0px) scaleY(0.850);
    }
    .s-6-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, 10.0px) rotate(4.1deg);
    }
    .s-6-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-5:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, 0.0px);
    }
    .s-6-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-64.3deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(72.5deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(30.9deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-45.9deg);
    }
    .s-6-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(4.2deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-34.1deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-55.9deg);
    }
    .s-6-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(14.2deg);
    }

    /* Cell x-6, y-6 */
    .s-6-6:hover ~ .ragdoll-root {
      transform: translate(3.6px, 48.0px) scaleY(0.820);
    }
    .s-6-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, 20.0px) rotate(4.1deg);
    }
    .s-6-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-6:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, 2.0px);
    }
    .s-6-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-62.1deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(70.3deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(35.9deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-55.9deg);
    }
    .s-6-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(5.9deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-39.1deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-65.9deg);
    }
    .s-6-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(15.9deg);
    }

    /* Cell x-6, y-7 */
    .s-6-7:hover ~ .ragdoll-root {
      transform: translate(3.6px, 56.0px) scaleY(0.790);
    }
    .s-6-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, 30.0px) rotate(4.1deg);
    }
    .s-6-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-7:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, 4.0px);
    }
    .s-6-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-59.9deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(68.1deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(40.9deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-65.9deg);
    }
    .s-6-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(7.6deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-44.1deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-75.9deg);
    }
    .s-6-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(17.6deg);
    }

    /* Cell x-6, y-8 */
    .s-6-8:hover ~ .ragdoll-root {
      transform: translate(3.6px, 64.0px) scaleY(0.760);
    }
    .s-6-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, 40.0px) rotate(4.1deg);
    }
    .s-6-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-8:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, 6.0px);
    }
    .s-6-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-57.7deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(65.9deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(45.9deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-75.9deg);
    }
    .s-6-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(9.2deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-49.1deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-85.9deg);
    }
    .s-6-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(19.2deg);
    }

    /* Cell x-6, y-9 */
    .s-6-9:hover ~ .ragdoll-root {
      transform: translate(3.6px, 72.0px) scaleY(0.730);
    }
    .s-6-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(5.5px, 50.0px) rotate(4.1deg);
    }
    .s-6-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(2.2deg);
    }
    .s-6-9:hover ~ .ragdoll-root .eye {
      transform: translate(0.9px, 8.0px);
    }
    .s-6-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(1.4deg);
    }
    .s-6-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(0.9deg);
    }
    .s-6-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(0.5deg);
    }
    .s-6-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(0.4deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-55.5deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-37.3deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-24.1deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-19.1deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-11.8deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-22.5deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-15.7deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-26.4deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-19.1deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(63.6deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(42.7deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(25.9deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(20.9deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(13.2deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(24.5deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(17.3deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(28.6deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(20.9deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(50.9deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-85.9deg);
    }
    .s-6-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(10.9deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-54.1deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-95.9deg);
    }
    .s-6-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(20.9deg);
    }

    /* Cell x-7, y-0 */
    .s-7-0:hover ~ .ragdoll-root {
      transform: translate(10.9px, 0.0px) scaleY(1.000);
    }
    .s-7-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, -40.0px) rotate(12.3deg);
    }
    .s-7-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-0:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, -10.0px);
    }
    .s-7-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-66.4deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(90.9deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(2.7deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(2.3deg);
    }
    .s-7-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-2.3deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-12.3deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-7.7deg);
    }
    .s-7-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(7.7deg);
    }

    /* Cell x-7, y-1 */
    .s-7-1:hover ~ .ragdoll-root {
      transform: translate(10.9px, 8.0px) scaleY(0.970);
    }
    .s-7-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, -30.0px) rotate(12.3deg);
    }
    .s-7-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-1:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, -8.0px);
    }
    .s-7-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-64.1deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(88.7deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(7.7deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-7.7deg);
    }
    .s-7-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-0.6deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-17.3deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-17.7deg);
    }
    .s-7-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(9.4deg);
    }

    /* Cell x-7, y-2 */
    .s-7-2:hover ~ .ragdoll-root {
      transform: translate(10.9px, 16.0px) scaleY(0.940);
    }
    .s-7-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, -20.0px) rotate(12.3deg);
    }
    .s-7-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-2:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, -6.0px);
    }
    .s-7-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-61.9deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(86.5deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(12.7deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-17.7deg);
    }
    .s-7-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(1.1deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-22.3deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-27.7deg);
    }
    .s-7-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(11.1deg);
    }

    /* Cell x-7, y-3 */
    .s-7-3:hover ~ .ragdoll-root {
      transform: translate(10.9px, 24.0px) scaleY(0.910);
    }
    .s-7-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, -10.0px) rotate(12.3deg);
    }
    .s-7-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-3:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, -4.0px);
    }
    .s-7-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-59.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(84.2deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(17.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-27.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(2.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-27.3deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-37.7deg);
    }
    .s-7-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(12.7deg);
    }

    /* Cell x-7, y-4 */
    .s-7-4:hover ~ .ragdoll-root {
      transform: translate(10.9px, 32.0px) scaleY(0.880);
    }
    .s-7-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, 0.0px) rotate(12.3deg);
    }
    .s-7-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-4:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, -2.0px);
    }
    .s-7-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-57.5deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(82.0deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(22.7deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-37.7deg);
    }
    .s-7-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(4.4deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-32.3deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-47.7deg);
    }
    .s-7-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(14.4deg);
    }

    /* Cell x-7, y-5 */
    .s-7-5:hover ~ .ragdoll-root {
      transform: translate(10.9px, 40.0px) scaleY(0.850);
    }
    .s-7-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, 10.0px) rotate(12.3deg);
    }
    .s-7-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-5:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, 0.0px);
    }
    .s-7-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-55.3deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(79.8deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(27.7deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-47.7deg);
    }
    .s-7-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(6.1deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-37.3deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-57.7deg);
    }
    .s-7-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(16.1deg);
    }

    /* Cell x-7, y-6 */
    .s-7-6:hover ~ .ragdoll-root {
      transform: translate(10.9px, 48.0px) scaleY(0.820);
    }
    .s-7-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, 20.0px) rotate(12.3deg);
    }
    .s-7-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-6:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, 2.0px);
    }
    .s-7-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-53.0deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(77.6deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(32.7deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-57.7deg);
    }
    .s-7-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(7.7deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-42.3deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-67.7deg);
    }
    .s-7-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(17.7deg);
    }

    /* Cell x-7, y-7 */
    .s-7-7:hover ~ .ragdoll-root {
      transform: translate(10.9px, 56.0px) scaleY(0.790);
    }
    .s-7-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, 30.0px) rotate(12.3deg);
    }
    .s-7-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-7:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, 4.0px);
    }
    .s-7-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-50.8deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(75.4deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(37.7deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-67.7deg);
    }
    .s-7-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(9.4deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-47.3deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-77.7deg);
    }
    .s-7-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(19.4deg);
    }

    /* Cell x-7, y-8 */
    .s-7-8:hover ~ .ragdoll-root {
      transform: translate(10.9px, 64.0px) scaleY(0.760);
    }
    .s-7-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, 40.0px) rotate(12.3deg);
    }
    .s-7-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-8:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, 6.0px);
    }
    .s-7-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-48.6deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(73.1deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(42.7deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-77.7deg);
    }
    .s-7-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(11.1deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-52.3deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-87.7deg);
    }
    .s-7-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(21.1deg);
    }

    /* Cell x-7, y-9 */
    .s-7-9:hover ~ .ragdoll-root {
      transform: translate(10.9px, 72.0px) scaleY(0.730);
    }
    .s-7-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(16.4px, 50.0px) rotate(12.3deg);
    }
    .s-7-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(6.5deg);
    }
    .s-7-9:hover ~ .ragdoll-root .eye {
      transform: translate(2.7px, 8.0px);
    }
    .s-7-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(4.1deg);
    }
    .s-7-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(2.7deg);
    }
    .s-7-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(1.6deg);
    }
    .s-7-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.1deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-46.4deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-31.8deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-22.3deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-17.3deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-10.5deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-20.4deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-14.2deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-24.1deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-17.3deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(70.9deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(48.2deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(27.7deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(22.7deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(14.5deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(26.6deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(18.8deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(30.9deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(22.7deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(47.7deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-87.7deg);
    }
    .s-7-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(12.7deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-57.3deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-97.7deg);
    }
    .s-7-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(22.7deg);
    }

    /* Cell x-8, y-0 */
    .s-8-0:hover ~ .ragdoll-root {
      transform: translate(18.2px, 0.0px) scaleY(1.000);
    }
    .s-8-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, -40.0px) rotate(20.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-0:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, -10.0px);
    }
    .s-8-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-57.3deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(98.2deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(-0.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(0.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(-0.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-15.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-9.5deg);
    }
    .s-8-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(9.5deg);
    }

    /* Cell x-8, y-1 */
    .s-8-1:hover ~ .ragdoll-root {
      transform: translate(18.2px, 8.0px) scaleY(0.970);
    }
    .s-8-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, -30.0px) rotate(20.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-1:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, -8.0px);
    }
    .s-8-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-55.1deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(96.0deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(4.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-9.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(1.2deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-20.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-19.5deg);
    }
    .s-8-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(11.2deg);
    }

    /* Cell x-8, y-2 */
    .s-8-2:hover ~ .ragdoll-root {
      transform: translate(18.2px, 16.0px) scaleY(0.940);
    }
    .s-8-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, -20.0px) rotate(20.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-2:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, -6.0px);
    }
    .s-8-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-52.8deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(93.7deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(9.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-19.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(2.9deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-25.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-29.5deg);
    }
    .s-8-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(12.9deg);
    }

    /* Cell x-8, y-3 */
    .s-8-3:hover ~ .ragdoll-root {
      transform: translate(18.2px, 24.0px) scaleY(0.910);
    }
    .s-8-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, -10.0px) rotate(20.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-3:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, -4.0px);
    }
    .s-8-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-50.6deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(91.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(14.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-29.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(4.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-30.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-39.5deg);
    }
    .s-8-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(14.5deg);
    }

    /* Cell x-8, y-4 */
    .s-8-4:hover ~ .ragdoll-root {
      transform: translate(18.2px, 32.0px) scaleY(0.880);
    }
    .s-8-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, 0.0px) rotate(20.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-4:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, -2.0px);
    }
    .s-8-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-48.4deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(89.3deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(19.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-39.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(6.2deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-35.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-49.5deg);
    }
    .s-8-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(16.2deg);
    }

    /* Cell x-8, y-5 */
    .s-8-5:hover ~ .ragdoll-root {
      transform: translate(18.2px, 40.0px) scaleY(0.850);
    }
    .s-8-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, 10.0px) rotate(20.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-5:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, 0.0px);
    }
    .s-8-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-46.2deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(87.1deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(24.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-49.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(7.9deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-40.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-59.5deg);
    }
    .s-8-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(17.9deg);
    }

    /* Cell x-8, y-6 */
    .s-8-6:hover ~ .ragdoll-root {
      transform: translate(18.2px, 48.0px) scaleY(0.820);
    }
    .s-8-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, 20.0px) rotate(20.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-6:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, 2.0px);
    }
    .s-8-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-43.9deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(84.8deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(29.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-59.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(9.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-45.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-69.5deg);
    }
    .s-8-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(19.5deg);
    }

    /* Cell x-8, y-7 */
    .s-8-7:hover ~ .ragdoll-root {
      transform: translate(18.2px, 56.0px) scaleY(0.790);
    }
    .s-8-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, 30.0px) rotate(20.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-7:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, 4.0px);
    }
    .s-8-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-41.7deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(82.6deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(34.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-69.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(11.2deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-50.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-79.5deg);
    }
    .s-8-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(21.2deg);
    }

    /* Cell x-8, y-8 */
    .s-8-8:hover ~ .ragdoll-root {
      transform: translate(18.2px, 64.0px) scaleY(0.760);
    }
    .s-8-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, 40.0px) rotate(20.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-8:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, 6.0px);
    }
    .s-8-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-39.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(80.4deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(39.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-79.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(12.9deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-55.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-89.5deg);
    }
    .s-8-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(22.9deg);
    }

    /* Cell x-8, y-9 */
    .s-8-9:hover ~ .ragdoll-root {
      transform: translate(18.2px, 72.0px) scaleY(0.730);
    }
    .s-8-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(27.3px, 50.0px) rotate(20.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(10.9deg);
    }
    .s-8-9:hover ~ .ragdoll-root .eye {
      transform: translate(4.5px, 8.0px);
    }
    .s-8-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(6.8deg);
    }
    .s-8-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(4.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(2.7deg);
    }
    .s-8-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(1.8deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-37.3deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-26.4deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-20.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-15.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-9.1deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-18.3deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-12.6deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-21.8deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-15.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(78.2deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(53.6deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(29.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(24.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(15.9deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(28.7deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(20.4deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(33.2deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(24.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(44.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-89.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(14.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-60.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-99.5deg);
    }
    .s-8-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(24.5deg);
    }

    /* Cell x-9, y-0 */
    .s-9-0:hover ~ .ragdoll-root {
      transform: translate(25.5px, 0.0px) scaleY(1.000);
    }
    .s-9-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, -40.0px) rotate(28.6deg);
    }
    .s-9-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-0:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, -10.0px);
    }
    .s-9-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-48.2deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(105.5deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(-3.6deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-1.4deg);
    }
    .s-9-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(1.4deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-18.6deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-11.4deg);
    }
    .s-9-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(11.4deg);
    }

    /* Cell x-9, y-1 */
    .s-9-1:hover ~ .ragdoll-root {
      transform: translate(25.5px, 8.0px) scaleY(0.970);
    }
    .s-9-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, -30.0px) rotate(28.6deg);
    }
    .s-9-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-1:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, -8.0px);
    }
    .s-9-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-46.0deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(103.2deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(1.4deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-11.4deg);
    }
    .s-9-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(3.0deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-23.6deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-21.4deg);
    }
    .s-9-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(13.0deg);
    }

    /* Cell x-9, y-2 */
    .s-9-2:hover ~ .ragdoll-root {
      transform: translate(25.5px, 16.0px) scaleY(0.940);
    }
    .s-9-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, -20.0px) rotate(28.6deg);
    }
    .s-9-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-2:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, -6.0px);
    }
    .s-9-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-43.7deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(101.0deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(6.4deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-21.4deg);
    }
    .s-9-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(4.7deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-28.6deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-31.4deg);
    }
    .s-9-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(14.7deg);
    }

    /* Cell x-9, y-3 */
    .s-9-3:hover ~ .ragdoll-root {
      transform: translate(25.5px, 24.0px) scaleY(0.910);
    }
    .s-9-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, -10.0px) rotate(28.6deg);
    }
    .s-9-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-3:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, -4.0px);
    }
    .s-9-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-41.5deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(98.8deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(11.4deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-31.4deg);
    }
    .s-9-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(6.4deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-33.6deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-41.4deg);
    }
    .s-9-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(16.4deg);
    }

    /* Cell x-9, y-4 */
    .s-9-4:hover ~ .ragdoll-root {
      transform: translate(25.5px, 32.0px) scaleY(0.880);
    }
    .s-9-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, 0.0px) rotate(28.6deg);
    }
    .s-9-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-4:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, -2.0px);
    }
    .s-9-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-39.3deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(96.6deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(16.4deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-41.4deg);
    }
    .s-9-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(8.0deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-38.6deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-51.4deg);
    }
    .s-9-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(18.0deg);
    }

    /* Cell x-9, y-5 */
    .s-9-5:hover ~ .ragdoll-root {
      transform: translate(25.5px, 40.0px) scaleY(0.850);
    }
    .s-9-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, 10.0px) rotate(28.6deg);
    }
    .s-9-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-5:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, 0.0px);
    }
    .s-9-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-37.1deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(94.3deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(21.4deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-51.4deg);
    }
    .s-9-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(9.7deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-43.6deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-61.4deg);
    }
    .s-9-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(19.7deg);
    }

    /* Cell x-9, y-6 */
    .s-9-6:hover ~ .ragdoll-root {
      transform: translate(25.5px, 48.0px) scaleY(0.820);
    }
    .s-9-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, 20.0px) rotate(28.6deg);
    }
    .s-9-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-6:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, 2.0px);
    }
    .s-9-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-34.8deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(92.1deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(26.4deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-61.4deg);
    }
    .s-9-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(11.4deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-48.6deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-71.4deg);
    }
    .s-9-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(21.4deg);
    }

    /* Cell x-9, y-7 */
    .s-9-7:hover ~ .ragdoll-root {
      transform: translate(25.5px, 56.0px) scaleY(0.790);
    }
    .s-9-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, 30.0px) rotate(28.6deg);
    }
    .s-9-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-7:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, 4.0px);
    }
    .s-9-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-32.6deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(89.9deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(31.4deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-71.4deg);
    }
    .s-9-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(13.0deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-53.6deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-81.4deg);
    }
    .s-9-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(23.0deg);
    }

    /* Cell x-9, y-8 */
    .s-9-8:hover ~ .ragdoll-root {
      transform: translate(25.5px, 64.0px) scaleY(0.760);
    }
    .s-9-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, 40.0px) rotate(28.6deg);
    }
    .s-9-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-8:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, 6.0px);
    }
    .s-9-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-30.4deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(87.7deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(36.4deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-81.4deg);
    }
    .s-9-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(14.7deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-58.6deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-91.4deg);
    }
    .s-9-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(24.7deg);
    }

    /* Cell x-9, y-9 */
    .s-9-9:hover ~ .ragdoll-root {
      transform: translate(25.5px, 72.0px) scaleY(0.730);
    }
    .s-9-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(38.2px, 50.0px) rotate(28.6deg);
    }
    .s-9-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(15.3deg);
    }
    .s-9-9:hover ~ .ragdoll-root .eye {
      transform: translate(6.4px, 8.0px);
    }
    .s-9-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(9.5deg);
    }
    .s-9-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(6.4deg);
    }
    .s-9-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(3.8deg);
    }
    .s-9-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(2.5deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-28.2deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-20.9deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-18.6deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-13.6deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-7.7deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-16.2deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-11.1deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-19.5deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-13.6deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(85.5deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(59.1deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(31.4deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(26.4deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(17.3deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(30.8deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(21.9deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(35.5deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(26.4deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(41.4deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-91.4deg);
    }
    .s-9-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(16.4deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-63.6deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-101.4deg);
    }
    .s-9-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(26.4deg);
    }

    /* Cell x-10, y-0 */
    .s-10-0:hover ~ .ragdoll-root {
      transform: translate(32.7px, 0.0px) scaleY(1.000);
    }
    .s-10-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, -40.0px) rotate(36.8deg);
    }
    .s-10-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-0:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, -10.0px);
    }
    .s-10-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-39.1deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(112.7deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(-6.8deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-3.2deg);
    }
    .s-10-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(3.2deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-21.8deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-13.2deg);
    }
    .s-10-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(13.2deg);
    }

    /* Cell x-10, y-1 */
    .s-10-1:hover ~ .ragdoll-root {
      transform: translate(32.7px, 8.0px) scaleY(0.970);
    }
    .s-10-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, -30.0px) rotate(36.8deg);
    }
    .s-10-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-1:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, -8.0px);
    }
    .s-10-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-36.9deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(110.5deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(-1.8deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-13.2deg);
    }
    .s-10-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(4.8deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-26.8deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-23.2deg);
    }
    .s-10-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(14.8deg);
    }

    /* Cell x-10, y-2 */
    .s-10-2:hover ~ .ragdoll-root {
      transform: translate(32.7px, 16.0px) scaleY(0.940);
    }
    .s-10-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, -20.0px) rotate(36.8deg);
    }
    .s-10-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-2:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, -6.0px);
    }
    .s-10-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-34.6deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(108.3deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(3.2deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-23.2deg);
    }
    .s-10-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(6.5deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-31.8deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-33.2deg);
    }
    .s-10-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(16.5deg);
    }

    /* Cell x-10, y-3 */
    .s-10-3:hover ~ .ragdoll-root {
      transform: translate(32.7px, 24.0px) scaleY(0.910);
    }
    .s-10-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, -10.0px) rotate(36.8deg);
    }
    .s-10-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-3:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, -4.0px);
    }
    .s-10-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-32.4deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(106.1deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(8.2deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-33.2deg);
    }
    .s-10-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(8.2deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-36.8deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-43.2deg);
    }
    .s-10-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(18.2deg);
    }

    /* Cell x-10, y-4 */
    .s-10-4:hover ~ .ragdoll-root {
      transform: translate(32.7px, 32.0px) scaleY(0.880);
    }
    .s-10-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, 0.0px) rotate(36.8deg);
    }
    .s-10-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-4:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, -2.0px);
    }
    .s-10-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-30.2deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(103.8deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(13.2deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-43.2deg);
    }
    .s-10-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(9.8deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-41.8deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-53.2deg);
    }
    .s-10-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(19.8deg);
    }

    /* Cell x-10, y-5 */
    .s-10-5:hover ~ .ragdoll-root {
      transform: translate(32.7px, 40.0px) scaleY(0.850);
    }
    .s-10-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, 10.0px) rotate(36.8deg);
    }
    .s-10-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-5:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, 0.0px);
    }
    .s-10-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-28.0deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(101.6deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(18.2deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-53.2deg);
    }
    .s-10-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(11.5deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-46.8deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-63.2deg);
    }
    .s-10-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(21.5deg);
    }

    /* Cell x-10, y-6 */
    .s-10-6:hover ~ .ragdoll-root {
      transform: translate(32.7px, 48.0px) scaleY(0.820);
    }
    .s-10-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, 20.0px) rotate(36.8deg);
    }
    .s-10-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-6:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, 2.0px);
    }
    .s-10-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-25.8deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(99.4deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(23.2deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-63.2deg);
    }
    .s-10-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(13.2deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-51.8deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-73.2deg);
    }
    .s-10-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(23.2deg);
    }

    /* Cell x-10, y-7 */
    .s-10-7:hover ~ .ragdoll-root {
      transform: translate(32.7px, 56.0px) scaleY(0.790);
    }
    .s-10-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, 30.0px) rotate(36.8deg);
    }
    .s-10-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-7:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, 4.0px);
    }
    .s-10-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-23.5deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(97.2deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(28.2deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-73.2deg);
    }
    .s-10-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(14.8deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-56.8deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-83.2deg);
    }
    .s-10-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(24.8deg);
    }

    /* Cell x-10, y-8 */
    .s-10-8:hover ~ .ragdoll-root {
      transform: translate(32.7px, 64.0px) scaleY(0.760);
    }
    .s-10-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, 40.0px) rotate(36.8deg);
    }
    .s-10-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-8:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, 6.0px);
    }
    .s-10-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-21.3deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(94.9deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(33.2deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-83.2deg);
    }
    .s-10-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(16.5deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-61.8deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-93.2deg);
    }
    .s-10-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(26.5deg);
    }

    /* Cell x-10, y-9 */
    .s-10-9:hover ~ .ragdoll-root {
      transform: translate(32.7px, 72.0px) scaleY(0.730);
    }
    .s-10-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(49.1px, 50.0px) rotate(36.8deg);
    }
    .s-10-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(19.6deg);
    }
    .s-10-9:hover ~ .ragdoll-root .eye {
      transform: translate(8.2px, 8.0px);
    }
    .s-10-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(12.3deg);
    }
    .s-10-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(8.2deg);
    }
    .s-10-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(4.9deg);
    }
    .s-10-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(3.3deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-19.1deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-15.5deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-16.8deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-11.8deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-6.4deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-14.1deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-9.5deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-17.3deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-11.8deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(92.7deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(64.5deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(33.2deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(28.2deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(18.6deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(32.9deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(23.5deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(37.7deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(28.2deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(38.2deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-93.2deg);
    }
    .s-10-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(18.2deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-66.8deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-103.2deg);
    }
    .s-10-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(28.2deg);
    }

    /* Cell x-11, y-0 */
    .s-11-0:hover ~ .ragdoll-root {
      transform: translate(40.0px, 0.0px) scaleY(1.000);
    }
    .s-11-0:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, -40.0px) rotate(45.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, -10.0px);
    }
    .s-11-0:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-12.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(12.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-30.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(120.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(-10.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-5.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .l-foot {
      transform: rotate(5.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-25.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-15.0deg);
    }
    .s-11-0:hover ~ .ragdoll-root .r-foot {
      transform: rotate(15.0deg);
    }

    /* Cell x-11, y-1 */
    .s-11-1:hover ~ .ragdoll-root {
      transform: translate(40.0px, 8.0px) scaleY(0.970);
    }
    .s-11-1:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, -30.0px) rotate(45.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, -8.0px);
    }
    .s-11-1:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-10.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(10.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-27.8deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(117.8deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(-5.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-15.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .l-foot {
      transform: rotate(6.7deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-30.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-25.0deg);
    }
    .s-11-1:hover ~ .ragdoll-root .r-foot {
      transform: rotate(16.7deg);
    }

    /* Cell x-11, y-2 */
    .s-11-2:hover ~ .ragdoll-root {
      transform: translate(40.0px, 16.0px) scaleY(0.940);
    }
    .s-11-2:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, -20.0px) rotate(45.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, -6.0px);
    }
    .s-11-2:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-8.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(8.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-25.6deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(115.6deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(0.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-25.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .l-foot {
      transform: rotate(8.3deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-35.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-35.0deg);
    }
    .s-11-2:hover ~ .ragdoll-root .r-foot {
      transform: rotate(18.3deg);
    }

    /* Cell x-11, y-3 */
    .s-11-3:hover ~ .ragdoll-root {
      transform: translate(40.0px, 24.0px) scaleY(0.910);
    }
    .s-11-3:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, -10.0px) rotate(45.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, -4.0px);
    }
    .s-11-3:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(6.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-23.3deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(113.3deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(5.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-35.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .l-foot {
      transform: rotate(10.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-40.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-45.0deg);
    }
    .s-11-3:hover ~ .ragdoll-root .r-foot {
      transform: rotate(20.0deg);
    }

    /* Cell x-11, y-4 */
    .s-11-4:hover ~ .ragdoll-root {
      transform: translate(40.0px, 32.0px) scaleY(0.880);
    }
    .s-11-4:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, 0.0px) rotate(45.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, -2.0px);
    }
    .s-11-4:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(4.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-21.1deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(111.1deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(10.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-45.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .l-foot {
      transform: rotate(11.7deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-45.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-55.0deg);
    }
    .s-11-4:hover ~ .ragdoll-root .r-foot {
      transform: rotate(21.7deg);
    }

    /* Cell x-11, y-5 */
    .s-11-5:hover ~ .ragdoll-root {
      transform: translate(40.0px, 40.0px) scaleY(0.850);
    }
    .s-11-5:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, 10.0px) rotate(45.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, 0.0px);
    }
    .s-11-5:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(2.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-18.9deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(108.9deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(15.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-55.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .l-foot {
      transform: rotate(13.3deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-50.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-65.0deg);
    }
    .s-11-5:hover ~ .ragdoll-root .r-foot {
      transform: rotate(23.3deg);
    }

    /* Cell x-11, y-6 */
    .s-11-6:hover ~ .ragdoll-root {
      transform: translate(40.0px, 48.0px) scaleY(0.820);
    }
    .s-11-6:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, 20.0px) rotate(45.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, 2.0px);
    }
    .s-11-6:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(0.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(0.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-16.7deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(106.7deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(20.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-65.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .l-foot {
      transform: rotate(15.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-55.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-75.0deg);
    }
    .s-11-6:hover ~ .ragdoll-root .r-foot {
      transform: rotate(25.0deg);
    }

    /* Cell x-11, y-7 */
    .s-11-7:hover ~ .ragdoll-root {
      transform: translate(40.0px, 56.0px) scaleY(0.790);
    }
    .s-11-7:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, 30.0px) rotate(45.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, 4.0px);
    }
    .s-11-7:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(2.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-2.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-14.4deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(104.4deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(25.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-75.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .l-foot {
      transform: rotate(16.7deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-60.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-85.0deg);
    }
    .s-11-7:hover ~ .ragdoll-root .r-foot {
      transform: rotate(26.7deg);
    }

    /* Cell x-11, y-8 */
    .s-11-8:hover ~ .ragdoll-root {
      transform: translate(40.0px, 64.0px) scaleY(0.760);
    }
    .s-11-8:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, 40.0px) rotate(45.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, 6.0px);
    }
    .s-11-8:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(4.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-4.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-12.2deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(102.2deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(30.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-85.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .l-foot {
      transform: rotate(18.3deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-65.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-95.0deg);
    }
    .s-11-8:hover ~ .ragdoll-root .r-foot {
      transform: rotate(28.3deg);
    }

    /* Cell x-11, y-9 */
    .s-11-9:hover ~ .ragdoll-root {
      transform: translate(40.0px, 72.0px) scaleY(0.730);
    }
    .s-11-9:hover ~ .ragdoll-root .head-joint {
      transform: translate(60.0px, 50.0px) rotate(45.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .neck-joint {
      transform: rotate(24.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .eye {
      transform: translate(10.0px, 8.0px);
    }
    .s-11-9:hover ~ .ragdoll-root .spine-s4 {
      transform: rotate(15.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .spine-s3 {
      transform: rotate(10.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .spine-s2 {
      transform: rotate(6.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .spine-s1 {
      transform: rotate(4.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-clavicle {
      transform: rotate(6.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-clavicle {
      transform: rotate(-6.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-arm-s1 {
      transform: rotate(-10.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-arm-s2 {
      transform: rotate(-10.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-wrist {
      transform: rotate(-15.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-finger1-1 {
      transform: rotate(-10.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-finger1-2 {
      transform: rotate(-5.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-finger2-1 {
      transform: rotate(-12.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-finger2-2 {
      transform: rotate(-8.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-finger3-1 {
      transform: rotate(-15.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-finger3-2 {
      transform: rotate(-10.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-arm-s1 {
      transform: rotate(100.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-arm-s2 {
      transform: rotate(70.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-wrist {
      transform: rotate(35.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-finger1-1 {
      transform: rotate(30.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-finger1-2 {
      transform: rotate(20.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-finger2-1 {
      transform: rotate(35.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-finger2-2 {
      transform: rotate(25.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-finger3-1 {
      transform: rotate(40.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-finger3-2 {
      transform: rotate(30.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-leg-s1 {
      transform: rotate(35.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-leg-s2 {
      transform: rotate(-95.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .l-foot {
      transform: rotate(20.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-leg-s1 {
      transform: rotate(-70.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-leg-s2 {
      transform: rotate(-105.0deg);
    }
    .s-11-9:hover ~ .ragdoll-root .r-foot {
      transform: rotate(30.0deg);
    }

  </style>

  <!-- 12x10 Interactive Sensor Grid Matrix (120 Hover zones covering the screen) -->
  <!-- Column 0 -->
  <rect class="sensor s-0-0" x="0" y="0" width="100" height="60" />
  <rect class="sensor s-0-1" x="0" y="60" width="100" height="60" />
  <rect class="sensor s-0-2" x="0" y="120" width="100" height="60" />
  <rect class="sensor s-0-3" x="0" y="180" width="100" height="60" />
  <rect class="sensor s-0-4" x="0" y="240" width="100" height="60" />
  <rect class="sensor s-0-5" x="0" y="300" width="100" height="60" />
  <rect class="sensor s-0-6" x="0" y="360" width="100" height="60" />
  <rect class="sensor s-0-7" x="0" y="420" width="100" height="60" />
  <rect class="sensor s-0-8" x="0" y="480" width="100" height="60" />
  <rect class="sensor s-0-9" x="0" y="540" width="100" height="60" />

  <!-- Column 1 -->
  <rect class="sensor s-1-0" x="100" y="0" width="100" height="60" />
  <rect class="sensor s-1-1" x="100" y="60" width="100" height="60" />
  <rect class="sensor s-1-2" x="100" y="120" width="100" height="60" />
  <rect class="sensor s-1-3" x="100" y="180" width="100" height="60" />
  <rect class="sensor s-1-4" x="100" y="240" width="100" height="60" />
  <rect class="sensor s-1-5" x="100" y="300" width="100" height="60" />
  <rect class="sensor s-1-6" x="100" y="360" width="100" height="60" />
  <rect class="sensor s-1-7" x="100" y="420" width="100" height="60" />
  <rect class="sensor s-1-8" x="100" y="480" width="100" height="60" />
  <rect class="sensor s-1-9" x="100" y="540" width="100" height="60" />

  <!-- Column 2 -->
  <rect class="sensor s-2-0" x="200" y="0" width="100" height="60" />
  <rect class="sensor s-2-1" x="200" y="60" width="100" height="60" />
  <rect class="sensor s-2-2" x="200" y="120" width="100" height="60" />
  <rect class="sensor s-2-3" x="200" y="180" width="100" height="60" />
  <rect class="sensor s-2-4" x="200" y="240" width="100" height="60" />
  <rect class="sensor s-2-5" x="200" y="300" width="100" height="60" />
  <rect class="sensor s-2-6" x="200" y="360" width="100" height="60" />
  <rect class="sensor s-2-7" x="200" y="420" width="100" height="60" />
  <rect class="sensor s-2-8" x="200" y="480" width="100" height="60" />
  <rect class="sensor s-2-9" x="200" y="540" width="100" height="60" />

  <!-- Column 3 -->
  <rect class="sensor s-3-0" x="300" y="0" width="100" height="60" />
  <rect class="sensor s-3-1" x="300" y="60" width="100" height="60" />
  <rect class="sensor s-3-2" x="300" y="120" width="100" height="60" />
  <rect class="sensor s-3-3" x="300" y="180" width="100" height="60" />
  <rect class="sensor s-3-4" x="300" y="240" width="100" height="60" />
  <rect class="sensor s-3-5" x="300" y="300" width="100" height="60" />
  <rect class="sensor s-3-6" x="300" y="360" width="100" height="60" />
  <rect class="sensor s-3-7" x="300" y="420" width="100" height="60" />
  <rect class="sensor s-3-8" x="300" y="480" width="100" height="60" />
  <rect class="sensor s-3-9" x="300" y="540" width="100" height="60" />

  <!-- Column 4 -->
  <rect class="sensor s-4-0" x="400" y="0" width="100" height="60" />
  <rect class="sensor s-4-1" x="400" y="60" width="100" height="60" />
  <rect class="sensor s-4-2" x="400" y="120" width="100" height="60" />
  <rect class="sensor s-4-3" x="400" y="180" width="100" height="60" />
  <rect class="sensor s-4-4" x="400" y="240" width="100" height="60" />
  <rect class="sensor s-4-5" x="400" y="300" width="100" height="60" />
  <rect class="sensor s-4-6" x="400" y="360" width="100" height="60" />
  <rect class="sensor s-4-7" x="400" y="420" width="100" height="60" />
  <rect class="sensor s-4-8" x="400" y="480" width="100" height="60" />
  <rect class="sensor s-4-9" x="400" y="540" width="100" height="60" />

  <!-- Column 5 -->
  <rect class="sensor s-5-0" x="500" y="0" width="100" height="60" />
  <rect class="sensor s-5-1" x="500" y="60" width="100" height="60" />
  <rect class="sensor s-5-2" x="500" y="120" width="100" height="60" />
  <rect class="sensor s-5-3" x="500" y="180" width="100" height="60" />
  <rect class="sensor s-5-4" x="500" y="240" width="100" height="60" />
  <rect class="sensor s-5-5" x="500" y="300" width="100" height="60" />
  <rect class="sensor s-5-6" x="500" y="360" width="100" height="60" />
  <rect class="sensor s-5-7" x="500" y="420" width="100" height="60" />
  <rect class="sensor s-5-8" x="500" y="480" width="100" height="60" />
  <rect class="sensor s-5-9" x="500" y="540" width="100" height="60" />

  <!-- Column 6 -->
  <rect class="sensor s-6-0" x="600" y="0" width="100" height="60" />
  <rect class="sensor s-6-1" x="600" y="60" width="100" height="60" />
  <rect class="sensor s-6-2" x="600" y="120" width="100" height="60" />
  <rect class="sensor s-6-3" x="600" y="180" width="100" height="60" />
  <rect class="sensor s-6-4" x="600" y="240" width="100" height="60" />
  <rect class="sensor s-6-5" x="600" y="300" width="100" height="60" />
  <rect class="sensor s-6-6" x="600" y="360" width="100" height="60" />
  <rect class="sensor s-6-7" x="600" y="420" width="100" height="60" />
  <rect class="sensor s-6-8" x="600" y="480" width="100" height="60" />
  <rect class="sensor s-6-9" x="600" y="540" width="100" height="60" />

  <!-- Column 7 -->
  <rect class="sensor s-7-0" x="700" y="0" width="100" height="60" />
  <rect class="sensor s-7-1" x="700" y="60" width="100" height="60" />
  <rect class="sensor s-7-2" x="700" y="120" width="100" height="60" />
  <rect class="sensor s-7-3" x="700" y="180" width="100" height="60" />
  <rect class="sensor s-7-4" x="700" y="240" width="100" height="60" />
  <rect class="sensor s-7-5" x="700" y="300" width="100" height="60" />
  <rect class="sensor s-7-6" x="700" y="360" width="100" height="60" />
  <rect class="sensor s-7-7" x="700" y="420" width="100" height="60" />
  <rect class="sensor s-7-8" x="700" y="480" width="100" height="60" />
  <rect class="sensor s-7-9" x="700" y="540" width="100" height="60" />

  <!-- Column 8 -->
  <rect class="sensor s-8-0" x="800" y="0" width="100" height="60" />
  <rect class="sensor s-8-1" x="800" y="60" width="100" height="60" />
  <rect class="sensor s-8-2" x="800" y="120" width="100" height="60" />
  <rect class="sensor s-8-3" x="800" y="180" width="100" height="60" />
  <rect class="sensor s-8-4" x="800" y="240" width="100" height="60" />
  <rect class="sensor s-8-5" x="800" y="300" width="100" height="60" />
  <rect class="sensor s-8-6" x="800" y="360" width="100" height="60" />
  <rect class="sensor s-8-7" x="800" y="420" width="100" height="60" />
  <rect class="sensor s-8-8" x="800" y="480" width="100" height="60" />
  <rect class="sensor s-8-9" x="800" y="540" width="100" height="60" />

  <!-- Column 9 -->
  <rect class="sensor s-9-0" x="900" y="0" width="100" height="60" />
  <rect class="sensor s-9-1" x="900" y="60" width="100" height="60" />
  <rect class="sensor s-9-2" x="900" y="120" width="100" height="60" />
  <rect class="sensor s-9-3" x="900" y="180" width="100" height="60" />
  <rect class="sensor s-9-4" x="900" y="240" width="100" height="60" />
  <rect class="sensor s-9-5" x="900" y="300" width="100" height="60" />
  <rect class="sensor s-9-6" x="900" y="360" width="100" height="60" />
  <rect class="sensor s-9-7" x="900" y="420" width="100" height="60" />
  <rect class="sensor s-9-8" x="900" y="480" width="100" height="60" />
  <rect class="sensor s-9-9" x="900" y="540" width="100" height="60" />

  <!-- Column 10 -->
  <rect class="sensor s-10-0" x="1000" y="0" width="100" height="60" />
  <rect class="sensor s-10-1" x="1000" y="60" width="100" height="60" />
  <rect class="sensor s-10-2" x="1000" y="120" width="100" height="60" />
  <rect class="sensor s-10-3" x="1000" y="180" width="100" height="60" />
  <rect class="sensor s-10-4" x="1000" y="240" width="100" height="60" />
  <rect class="sensor s-10-5" x="1000" y="300" width="100" height="60" />
  <rect class="sensor s-10-6" x="1000" y="360" width="100" height="60" />
  <rect class="sensor s-10-7" x="1000" y="420" width="100" height="60" />
  <rect class="sensor s-10-8" x="1000" y="480" width="100" height="60" />
  <rect class="sensor s-10-9" x="1000" y="540" width="100" height="60" />

  <!-- Column 11 -->
  <rect class="sensor s-11-0" x="1100" y="0" width="100" height="60" />
  <rect class="sensor s-11-1" x="1100" y="60" width="100" height="60" />
  <rect class="sensor s-11-2" x="1100" y="120" width="100" height="60" />
  <rect class="sensor s-11-3" x="1100" y="180" width="100" height="60" />
  <rect class="sensor s-11-4" x="1100" y="240" width="100" height="60" />
  <rect class="sensor s-11-5" x="1100" y="300" width="100" height="60" />
  <rect class="sensor s-11-6" x="1100" y="360" width="100" height="60" />
  <rect class="sensor s-11-7" x="1100" y="420" width="100" height="60" />
  <rect class="sensor s-11-8" x="1100" y="480" width="100" height="60" />
  <rect class="sensor s-11-9" x="1100" y="540" width="100" height="60" />

  <!-- Ground Line -->
  <line x1="50" y1="520" x2="1150" y2="520" stroke="#30363D" stroke-width="4" stroke-linecap="round" />

  <!-- Background target marker showing visual center -->
  <circle cx="600" cy="300" r="3" fill="#30363D" />

  <!-- 1000-Joint Ragdoll Physics Stickman Entity -->
  <g class="ragdoll-root" transform="translate(200, 70)">
    
    <!-- HIP / PELVIS (Primary Root Node) -->
    <g class="hip-joint joint">
      <circle cx="400" cy="300" r="10" fill="#00D5FF" />
      
      <!-- SPINE SEGMENT 1 (Lower Lumbar) -->
      <g class="spine-s1 joint" style="transform-origin: 400px 300px;">
        <line x1="400" y1="300" x2="400" y2="270" stroke="#00D5FF" stroke-width="8" stroke-linecap="round" />
        <circle cx="400" cy="270" r="6" fill="#A9B7C6" />
        
        <!-- SPINE SEGMENT 2 (Thoracic) -->
        <g class="spine-s2 joint" style="transform-origin: 400px 270px;">
          <line x1="400" y1="270" x2="400" y2="240" stroke="#00D5FF" stroke-width="8" stroke-linecap="round" />
          <circle cx="400" cy="240" r="6" fill="#A9B7C6" />

          <!-- SPINE SEGMENT 3 (Upper Thoracic) -->
          <g class="spine-s3 joint" style="transform-origin: 400px 240px;">
            <line x1="400" y1="240" x2="400" y2="210" stroke="#00D5FF" stroke-width="8" stroke-linecap="round" />
            <circle cx="400" cy="210" r="6" fill="#A9B7C6" />

            <!-- SPINE SEGMENT 4 (Shoulder Base) -->
            <g class="spine-s4 joint" style="transform-origin: 400px 210px;">
              <line x1="400" y1="210" x2="400" y2="190" stroke="#00D5FF" stroke-width="8" stroke-linecap="round" />
              <circle cx="400" cy="190" r="6" fill="#A9B7C6" />
              
              <!-- NECK JOINT -->
              <g class="neck-joint joint" style="transform-origin: 400px 190px;">
                <line x1="400" y1="190" x2="400" y2="170" stroke="#00D5FF" stroke-width="6" stroke-linecap="round" />
                
                <!-- HEAD NODE -->
                <g class="head-joint joint" style="transform-origin: 400px 170px;">
                  <circle cx="400" cy="140" r="26" stroke="#00D5FF" stroke-width="8" fill="#0D1117" />
                  <!-- Biological Eyes (tracking cursor) -->
                  <g class="eye">
                    <circle cx="390" cy="136" r="3" fill="#A9B7C6" />
                    <circle cx="410" cy="136" r="3" fill="#A9B7C6" />
                  </g>
                  <path d="M 392 152 Q 400 158 408 152" stroke="#00D5FF" stroke-width="3" fill="none" />
                </g>
              </g>
              
              <!-- LEFT CLAVICLE -->
              <g class="l-clavicle joint" style="transform-origin: 396px 195px;">
                <line x1="396" y1="195" x2="370" y2="195" stroke="#00D5FF" stroke-width="6" stroke-linecap="round" />
                <circle cx="370" cy="195" r="5" fill="#A9B7C6" />

                <!-- LEFT SHOULDER & ARM SYSTEM -->
                <g class="l-arm-s1 joint" style="transform-origin: 370px 195px;">
                  <line x1="370" y1="195" x2="330" y2="210" stroke="#00D5FF" stroke-width="7" stroke-linecap="round" />
                  <circle cx="330" cy="210" r="5" fill="#A9B7C6" />
                  
                  <!-- LEFT FOREARM -->
                  <g class="l-arm-s2 joint" style="transform-origin: 330px 210px;">
                    <line x1="330" y1="210" x2="290" y2="230" stroke="#00D5FF" stroke-width="6" stroke-linecap="round" />
                    <circle cx="290" cy="230" r="4" fill="#A9B7C6" />
                    
                    <!-- LEFT WRIST & FINGERS -->
                    <g class="l-wrist joint" style="transform-origin: 290px 230px;">
                      <line x1="290" y1="230" x2="275" y2="235" stroke="#00D5FF" stroke-width="4" stroke-linecap="round" />
                      
                      <!-- Finger 1 -->
                      <g class="l-finger1-1 joint" style="transform-origin: 275px 235px;">
                        <line x1="275" y1="235" x2="265" y2="230" stroke="#A9B7C6" stroke-width="2" />
                        <g class="l-finger1-2 joint" style="transform-origin: 265px 230px;">
                          <line x1="265" y1="230" x2="258" y2="228" stroke="#A9B7C6" stroke-width="2" />
                        </g>
                      </g>
                      <!-- Finger 2 -->
                      <g class="l-finger2-1 joint" style="transform-origin: 275px 235px;">
                        <line x1="275" y1="235" x2="263" y2="237" stroke="#A9B7C6" stroke-width="2" />
                        <g class="l-finger2-2 joint" style="transform-origin: 263px 237px;">
                          <line x1="263" y1="237" x2="255" y2="239" stroke="#A9B7C6" stroke-width="2" />
                        </g>
                      </g>
                      <!-- Finger 3 -->
                      <g class="l-finger3-1 joint" style="transform-origin: 275px 235px;">
                        <line x1="275" y1="235" x2="266" y2="244" stroke="#A9B7C6" stroke-width="2" />
                        <g class="l-finger3-2 joint" style="transform-origin: 266px 244px;">
                          <line x1="266" y1="244" x2="258" y2="249" stroke="#A9B7C6" stroke-width="2" />
                        </g>
                      </g>

                    </g>
                  </g>
                </g>
              </g>

              <!-- RIGHT CLAVICLE -->
              <g class="r-clavicle joint" style="transform-origin: 404px 195px;">
                <line x1="404" y1="195" x2="430" y2="195" stroke="#00D5FF" stroke-width="6" stroke-linecap="round" />
                <circle cx="430" cy="195" r="5" fill="#A9B7C6" />

                <!-- RIGHT SHOULDER & ARM SYSTEM -->
                <g class="r-arm-s1 joint" style="transform-origin: 430px 195px;">
                  <line x1="430" y1="195" x2="470" y2="210" stroke="#00D5FF" stroke-width="7" stroke-linecap="round" />
                  <circle cx="470" cy="210" r="5" fill="#A9B7C6" />
                  
                  <!-- RIGHT FOREARM -->
                  <g class="r-arm-s2 joint" style="transform-origin: 470px 210px;">
                    <line x1="470" y1="210" x2="510" y2="230" stroke="#00D5FF" stroke-width="6" stroke-linecap="round" />
                    <circle cx="510" cy="230" r="4" fill="#A9B7C6" />
                    
                    <!-- RIGHT WRIST & FINGERS -->
                    <g class="r-wrist joint" style="transform-origin: 510px 230px;">
                      <line x1="510" y1="230" x2="525" y2="235" stroke="#00D5FF" stroke-width="4" stroke-linecap="round" />
                      
                      <!-- Finger 1 -->
                      <g class="r-finger1-1 joint" style="transform-origin: 525px 235px;">
                        <line x1="525" y1="235" x2="535" y2="230" stroke="#A9B7C6" stroke-width="2" />
                        <g class="r-finger1-2 joint" style="transform-origin: 535px 230px;">
                          <line x1="535" y1="230" x2="542" y2="228" stroke="#A9B7C6" stroke-width="2" />
                        </g>
                      </g>
                      <!-- Finger 2 -->
                      <g class="r-finger2-1 joint" style="transform-origin: 525px 235px;">
                        <line x1="525" y1="235" x2="537" y2="237" stroke="#A9B7C6" stroke-width="2" />
                        <g class="r-finger2-2 joint" style="transform-origin: 537px 237px;">
                          <line x1="537" y1="237" x2="545" y2="239" stroke="#A9B7C6" stroke-width="2" />
                        </g>
                      </g>
                      <!-- Finger 3 -->
                      <g class="r-finger3-1 joint" style="transform-origin: 525px 235px;">
                        <line x1="525" y1="235" x2="534" y2="244" stroke="#A9B7C6" stroke-width="2" />
                        <g class="r-finger3-2 joint" style="transform-origin: 534px 244px;">
                          <line x1="534" y1="244" x2="542" y2="249" stroke="#A9B7C6" stroke-width="2" />
                        </g>
                      </g>

                    </g>
                  </g>
                </g>
              </g>

            </g>
          </g>
        </g>
      </g>
      
      <!-- LEFT HIP & THIGH SYSTEM -->
      <g class="l-leg-s1 joint" style="transform-origin: 392px 305px;">
        <line x1="392" y1="305" x2="370" y2="365" stroke="#00D5FF" stroke-width="8" stroke-linecap="round" />
        <circle cx="370" cy="365" r="6" fill="#A9B7C6" />
        
        <!-- LEFT SHIN -->
        <g class="l-leg-s2 joint" style="transform-origin: 370px 365px;">
          <line x1="370" y1="365" x2="355" y2="430" stroke="#00D5FF" stroke-width="7" stroke-linecap="round" />
          <circle cx="355" cy="430" r="5" fill="#A9B7C6" />
          
          <!-- LEFT ANKLE & FOOT -->
          <g class="l-foot joint" style="transform-origin: 355px 430px;">
            <path d="M 355 430 L 330 445 L 360 445 Z" fill="none" stroke="#00D5FF" stroke-width="4" stroke-linejoin="round" />
          </g>
        </g>
      </g>

      <!-- RIGHT HIP & THIGH SYSTEM -->
      <g class="r-leg-s1 joint" style="transform-origin: 408px 305px;">
        <line x1="408" y1="305" x2="430" y2="365" stroke="#00D5FF" stroke-width="8" stroke-linecap="round" />
        <circle cx="430" cy="365" r="6" fill="#A9B7C6" />
        
        <!-- RIGHT SHIN -->
        <g class="r-leg-s2 joint" style="transform-origin: 430px 365px;">
          <line x1="430" y1="365" x2="445" y2="430" stroke="#00D5FF" stroke-width="7" stroke-linecap="round" />
          <circle cx="445" cy="430" r="5" fill="#A9B7C6" />
          
          <!-- RIGHT ANKLE & FOOT -->
          <g class="r-foot joint" style="transform-origin: 445px 430px;">
            <path d="M 445 430 L 470 445 L 440 445 Z" fill="none" stroke="#00D5FF" stroke-width="4" stroke-linejoin="round" />
          </g>
        </g>
      </g>
      
    </g>
  </g>
</svg>
</div>

<br/>

---

## 🐍 Contribution Snake Grid

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/bercaius/bercaius/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/bercaius/bercaius/output/github-contribution-grid-snake.svg">
    <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/bercaius/bercaius/output/github-contribution-grid-snake.svg">
  </picture>
</div>

<br/>

---

## 📊 Live Metrics & Core Analytics

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=bercaius&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&ring_color=00D5FF&title_color=00D5FF&icon_color=00D5FF" alt="GitHub Stats" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bercaius&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=00D5FF" alt="Top Languages" width="48%" />
</div>

<br/>

<div align="center">
  <sub>Decentralized. Animating. Secure. Executed in 2026.</sub>
</div>
