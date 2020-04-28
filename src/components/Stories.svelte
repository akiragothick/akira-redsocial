<script>
  const userimage =
    "https://scontent.flim10-1.fna.fbcdn.net/v/t1.0-1/cp0/p40x40/49656266_10213048896118671_4065369107543883776_n.jpg?_nc_cat=104&_nc_sid=dbb9e7&_nc_eui2=AeFimAcviGF6lXdzYlgyNQSaYPokoXeg3ztg-iShd6DfOyggz0xhh2W4IzDU37qwm_k&_nc_ohc=HptJ6RJVsF4AX-nryP2&_nc_ht=scontent.flim10-1.fna&oh=a14828d64b137481c65fa9d0b85c05ff&oe=5ECE307B";
</script>

<style>
  .Stories {
    border: 1px solid rgba(219, 219, 219, 1);
    border-radius: 4px;
    margin: 1em 0;
    padding: 0.5em 1em;
    background-color: white;
  }
  .Stories-item img {
    width: 32px;
    height: 32px;
    border-radius: 50%;
  }
  .Stories-item {
    display: flex;
    align-items: center;
    margin: 0 0 0.5em 0;
  }
  .Stories-item h2 {
    font-size: 14px;
    color: black;
    margin: 0 0 0 0.5em;
  }
  .Stories-item h2 span {
    display: block;
    font-size: 9px;
    text-transform: uppercase;
    color: gray;
  }
  .Stories-head {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.5em 0 0 0;
  }
  .Stories-head h2 {
    font-size: 12px;
    font-weight: 600;
  }
  .Stories-head span {
    font-size: 12px;
    font-weight: normal;
    color: black;
  }
  .Stories-items {
    margin: 0.5em 0 0.5em 0;
  }
  .Stories-item-box {
    width: 32px;
    height: 32px;
    border: double 2px transparent;
    border-radius: 100%;
    background-image: linear-gradient(#fff, #fff),
      radial-gradient(circle at top left, #f09433, #bc1888);
    background-origin: border-box;
    background-clip: content-box, border-box;
  }
</style>

<div class="Stories">
  <div class="Stories-container">
    <div class="Stories-head">
      <h2>Historias</h2>
      <span>Ver todas</span>
    </div>
    <div class="Stories-items">
      <div class="Stories-item">
        <div class="Stories-item-box">
          <img src={userimage} alt="" />
        </div>
        <h2>
          Grindelwald
          <span>Hace 1 hora</span>
        </h2>
      </div>
    </div>
  </div>
</div>
