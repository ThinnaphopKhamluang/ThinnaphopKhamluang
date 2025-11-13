<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>🐧 Penguin Animation</title>
<style>
  body {
    margin:0;
    height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    background:linear-gradient(#c9e9ff,#faffff);
    overflow:hidden;
  }

  .penguin {
    position:relative;
    width:100px;
    height:120px;
    animation:waddle 4s ease-in-out infinite;
  }

  /* ตัวเพนกวิน */
  .penguin .body {
    position:absolute;
    width:100%;
    height:100%;
    background:#0b1b2b;
    border-radius:50% 50% 40% 40%;
  }

  /* ท้อง */
  .penguin .belly {
    position:absolute;
    left:18px;
    top:20px;
    width:64px;
    height:80px;
    background:#fff;
    border-radius:50%;
  }

  /* ตา */
  .penguin .eye {
    position:absolute;
    width:10px;
    height:10px;
    background:#000;
    border-radius:50%;
    top:25px;
    animation:blink 4s infinite;
  }
  .penguin .eye.left { left:25px; }
  .penguin .eye.right { right:25px; }

  /* ปาก */
  .penguin .beak {
    position:absolute;
    width:20px;
    height:10px;
    background:#ffb347;
    border-radius:0 0 10px 10px;
    top:42px;
    left:40px;
  }

  /* ปีก */
  .penguin .wing {
    position:absolute;
    width:24px;
    height:50px;
    background:#071521;
    border-radius:50%;
    top:40px;
    animation:flap 3s ease-in-out infinite;
  }
  .penguin .wing.left { left:-12px; transform-origin:100% 0%; }
  .penguin .wing.right { right:-12px; transform-origin:0% 0%; }

  /* เท้า */
  .penguin .foot {
    position:absolute;
    width:28px;
    height:12px;
    background:#ffb347;
    bottom:0;
    border-radius:50% 50% 0 0;
  }
  .penguin .foot.left { left:20px; }
  .penguin .foot.right { right:20px; }

  /* Animation เคลื่อนไหว */
  @keyframes flap {
    0%,100% { transform:rotate(0deg

