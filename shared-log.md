HYDRA WORKSHOP at AAVISTUS FESTIVAL 2024

<https://hydra-hauptsachefrei-2023-workshop.glitch.me/#/>

///
FLOK JAM LINKS
<https://next.flok.cc/s/odd-crimson-magpie-68ee1578#>


NAOTO mail@naotohieda.com


Additional material
* another tutorial https://ccfest-2021-glitchme.glitch.me/
* Live coding tool list https://github.com/toplap/awesome-livecoding
  * https://strudel.cc/
* Discord community https://discord.com/invite/AdmeeJjFk6
* Hydra bot https://botsin.space/@hydra
* Hydra interactive documentation https://hydra.ojack.xyz/api/
* Hydra book https://hydra-book.glitch.me/#/
  * GLSL https://hydra-book.glitch.me/#/glsl
* examples made by hydra https://hydra.ojack.xyz/garden/
* hydra as module https://glitch.com/edit/#!/hydra-webpage
* image uploader https://imgbb.com/


speed=1
bpm=120

s0.initCam(0)
s0.initCam(1)
...

setResolution(640,480)


Code made by us

src(s0).rotate(3.14).out()

src(s0).rotate(1).add(osc().color(1,0,[1,0]),0.8).colorama().out()

noise(3.9,.1,.1).thresh(0.2).diff(osc(4.3)).diff(src(s0).modulate(o0).colorama(1)).out()

s0.initCam(1)

src(s0).blend(gradient(0.001,0.1)).colorama(0.01).diff(osc(10,0.00020)).modulate(noise(6), 0.001).out()

thingy = (shift = 0.0, noisefreq = 3.2, oscfreq = 6.2)

    => noise(noisefreq,.1).thresh(0.2).diff(osc(oscfreq,.1,shift));

thingy().modulate(thingy(),()=>Math.sin(time*-.001)).out()

Naoto (https://naotohieda.com/), Tallinn, https://www.youtube.com/watch?v=5iABNDvZ8IA

Hildar (https://www.sled.ee/home.html,https://katarinameister.weebly.com/ ) Helsinki (Tallinn originally), https://www.youtube.com/watch?v=qCljI3cIObU

Miranda (https://pulusound.fi), Helsinki, 
      ヤババイナ - さたぱんP feat. 初音ミク・重音テト・ずんだもん / YABABAINA - Satapan P feat.Miku Hatsune, Teto Kasane, Zundamon     https://www.youtube.com/watch?v=DDZtUUVJ0yc
feel free to join ALGORAVE HELSINKI :) https://discord.com/invite/fb7zk9av
we organize semi-regular meetups, workshops, concerts etc around music/visuals livecoding and other weird technological methods of making art

Markus (@mojmalimarki - https://www.instagram.com/mojmalimarki/), Helsinki, Amnesia Scanner - AS Over https://www.youtube.com/watch?v=cNpPs0gn5Mc

Ellen Sofie (https://www.instagram.com/ellensofieng/), Helsinki, can't think of anything sorry

Michael, from stockholm. Music video not sure havnt seen any good for a long time.

Otto (http://instagram.com/trsctr), Helsinki, Autechre - Gantz Graf

Sui (http://instagram.com/ssusui_), Riga/Helsinki
<3 MV
Max Cooper - Symphony in Acid (Official video by Ksawery Komputery)
https://www.youtube.com/watch?v=_n_iKR3Icio
Grimes ft. Janelle Monáe - Venus Fly
https://www.youtube.com/watch?v=eTLTXDHrgtw

Jan (@jbasandberg), Hanko, Video not sure, Noveller - No Dreams(?)

Artturi Elovirta https://www.instagram.com/artturielovirta/, Turku, Electro/techno

Reetta (ig: kahdeksasosa), Helsinki, 
Iñigo Montoya - Totem (https://www.youtube.com/watch?v=2pc43fnO5x8)

Patrik, Helsinki
Jamie xx - Gosh
https://youtu.be/hTGJfRPLe08?si=1gj2PfipVPxc43WA

Tigany (@tiganytigany), Helsinki, https://www.youtube.com/watch?v=8O7WTOkf2o8
Alejandro, (@alejo_end), from Panama City. Music Video Leftfield feat. Afrika Bambaataa - Afrika Shox (HD) (youtube.com)



// Passing HTML canvas to Hydra constructor

const canvas = document.createElement("CANVAS");

canvas.width = 800;
canvas.height = 800;
const hydra = new Hydra({
  canvas: canvas,
  detectAudio: false,
  enableStreamCapture: false,
  makeGlobal: true,
});
document.querySelector("#app").appendChild(canvas);

