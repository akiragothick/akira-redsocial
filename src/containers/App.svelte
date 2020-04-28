<script>
  import { onMount } from "svelte";
  import Header from "../components/Header.svelte";
  import Main from "./Main.svelte";
  import Timeline from "../components/Timeline.svelte";
  import Sidebar from "../components/Sidebar.svelte";

  let user = {
    nickname: "AkiraGothick",
    name: "Ernesto Vargas"
  };

  const userimage =
    "https://scontent.flim10-1.fna.fbcdn.net/v/t1.0-1/cp0/p40x40/49656266_10213048896118671_4065369107543883776_n.jpg?_nc_cat=104&_nc_sid=dbb9e7&_nc_eui2=AeFimAcviGF6lXdzYlgyNQSaYPokoXeg3ztg-iShd6DfOyggz0xhh2W4IzDU37qwm_k&_nc_ohc=HptJ6RJVsF4AX-nryP2&_nc_ht=scontent.flim10-1.fna&oh=a14828d64b137481c65fa9d0b85c05ff&oe=5ECE307B";

  let posts = [
    {
      username: user.nickname,
      avatar: userimage,
      location: "Perú",
      postComment: "¿Sabes qué es GIT?",
      photo:
        "https://scontent.flim10-1.fna.fbcdn.net/v/t1.0-9/92800380_10216451472140945_2720094043726938112_n.jpg?_nc_cat=106&_nc_sid=110474&_nc_eui2=AeH2ayLGEcmWseVG02NBDFeWy2QY7gX8DbPLZBjuBfwNs4TXyOFrXZh4nSsByN7SPm8&_nc_ohc=Xq3v-rGCY8IAX_p234Q&_nc_ht=scontent.flim10-1.fna&oh=e47bf5622da19e1eb93283482b7e1913&oe=5ECC04F6",
      comments: [
        {
          id: 1,
          username: user.nickname,
          text: "Estoy aprendiendo github"
        },
        {
          id: 2,
          username: "Grindelwald",
          text: "Es muy interesante"
        }
      ]
    },
    {
      username: "Grindelwald",
      avatar:
        "https://scontent.flim10-1.fna.fbcdn.net/v/t1.0-1/cp0/p50x50/87816834_2690213021025739_4684852229423759360_n.jpg?_nc_cat=104&_nc_sid=dbb9e7&_nc_eui2=AeFgTFpr4mky3eR6IvLm73E1HCzMPFpKyUIcLMw8WkrJQhcZP4G_ECYR9FdW7IoSmIQ&_nc_ohc=TTqMgtpfx5oAX_fkiuO&_nc_ht=scontent.flim10-1.fna&oh=3d0edc9aaadea0604c34eefa10461b12&oe=5ECBA415",
      location: "Perú",
      postComment: "#yomequedoencasa",
      photo:
        "https://scontent.flim10-1.fna.fbcdn.net/v/t1.0-9/92483372_591422158386397_753343835018362880_n.jpg?_nc_cat=111&_nc_sid=110474&_nc_eui2=AeGgO9l-vP_B1y1aWZP5NiC_Ee4VAgR6BXIR7hUCBHoFckX-n44Te--6ulUes9n7RPQ&_nc_ohc=N2iyHLBBqjMAX9QAUxE&_nc_ht=scontent.flim10-1.fna&oh=6df306f0adc2086c7a25c26b9fe95892&oe=5ECDA145",
      comments: [
        {
          id: 1,
          username: user.nickname,
          text: "Hahahha tu si ah"
        }
      ]
    }
  ];

  //   onMount(async () => {
  //     const response = await fetch(API);
  //     data = await response.json();
  //   });
</script>

<style>
  :global(body) {
    background-color: #fafafa;
    color: rgba(38, 38, 38, 0.7);
    font-family: "Lato", sans-serif;
    margin: 0;
    padding: 0;
  }
  :global(h1, h2, h3) {
    margin: 0;
    padding: 0;
  }
</style>

<Header />

<Main>
  <Timeline {posts} />
  <Sidebar {...user} />
</Main>
