<script>
  export let nickname;
  export let name;

  const userimage =
    "https://scontent.flim10-1.fna.fbcdn.net/v/t1.0-1/cp0/p40x40/49656266_10213048896118671_4065369107543883776_n.jpg?_nc_cat=104&_nc_sid=dbb9e7&_nc_eui2=AeFimAcviGF6lXdzYlgyNQSaYPokoXeg3ztg-iShd6DfOyggz0xhh2W4IzDU37qwm_k&_nc_ohc=HptJ6RJVsF4AX-nryP2&_nc_ht=scontent.flim10-1.fna&oh=a14828d64b137481c65fa9d0b85c05ff&oe=5ECE307B";
</script>

<style>
  .Profile-content {
    display: flex;
    align-items: center;
  }
  .Profile-avatar img {
    width: 42px;
    height: 42px;
    border-radius: 50%;
  }
  .Profile-info {
    margin: 0 0 0 0.5em;
  }
  .Profile-info h2 {
    font-size: 14px;
    color: black;
    margin: 0;
    padding: 0;
  }
  .Profile-info span {
    font-size: 12px;
    font-weight: normal;
  }
</style>

<div class="Profile">
  <div class="Profile-content">
    <div class="Profile-avatar">
      <img src={userimage} alt="" />
    </div>
    <div class="Profile-info">
      <h2>{nickname}</h2>
      <span>{name}</span>
    </div>
  </div>
</div>
