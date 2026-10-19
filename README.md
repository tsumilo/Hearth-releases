<p align="center">
  <img src="assets/banner.png" alt="Hearth: games with friends" width="100%">
</p>

<p align="center">
  <b>A launcher for the games we make</b>, for a small circle of friends.<br>
  <sub>Get a game in one click · keep it up to date · see who's online · open a lobby and play together</sub>
</p>

<p align="center"><img src="assets/divider.png" width="70%" alt=""></p>

<h2 align="center">Get Hearth</h2>

<p align="center">
  <a href="https://pub-0af611d981554c92b3dd76b8947076c5.r2.dev/launcher/Hearth-setup.exe"><img src="assets/btn-windows.png" width="300" alt="Download Hearth for Windows"></a>
</p>

<p align="center"><sub>
  Windows may say <i>Windows protected your PC</i>: click <i>More info</i>, then <i>Run anyway</i>.<br>
  Hearth is invite only: a friend who already has it gives you an invite code the first time you open it.
</sub></p>

<table align="center">
  <tr>
    <td align="center" width="25%"><b>One click</b><br><sub>Every game in one Library: get it, play it, and Hearth keeps it up to date</sub></td>
    <td align="center" width="25%"><b>Small, signed updates</b><br><sub>Downloads only the files that changed, and installs only releases signed by the Hearth key</sub></td>
    <td align="center" width="25%"><b>Friends &amp; lobbies</b><br><sub>See who's online and what they play, chat, and start a game together from a lobby</sub></td>
    <td align="center" width="25%"><b>Saves kept safe</b><br><sub>Your saves stay apart from the game, and Backups lets you go back to an older version</sub></td>
  </tr>
</table>

<p align="center"><img src="assets/divider.png" width="70%" alt=""></p>

<h2 align="center">The games</h2>

<table align="center">
  <tr>
    <td width="160" align="center"><img src="assets/game-kindle-and-keep.png" width="140" alt="Kindle &amp; Keep"></td>
    <td>
      <b>Kindle &amp; Keep</b> &nbsp;<sub>CO-OP BUILD &amp; DEFEND · 1–4 PLAYERS · IN THE WORKS</sub><br><br>
      Keep the hearthfire burning through the night. By day, build walls and towers inside the fire's light;
      when the dark comes, hold them together until dawn.<br>
      <sub>Made with Tinderbox, Hearth's own engine.</sub>
    </td>
  </tr>
</table>

<p align="center"><img src="assets/divider.png" width="70%" alt=""></p>

<details>
  <summary><b>What is in this repository</b></summary>
  <br>

  - `channels/`: the signed game lists Hearth reads (`stable`, and `beta` for testers).
  - The games' files and Hearth's installers are not in git: they are on Cloudflare R2 (the address is in each
    game list), one object per version of each file, named by its SHA-256.

  Hearth reads the game lists straight from `raw.githubusercontent.com`. A game list whose signature doesn't
  match the key built into Hearth is refused, and so is any file whose SHA-256 doesn't match the list. Hearth's
  own updates are signed too, with a key of their own.
</details>

<details>
  <summary><b>Privacy</b></summary>
  <br>

  - Game lists come from this repository on GitHub, and the files from Cloudflare R2, like any download.
  - With an invite, Hearth connects to the Hearth server for friends, chat and lobbies. The server keeps your
    chosen name, your friends list and your direct messages. Who's online, what they play, lobbies and lobby
    chat are only kept while the server runs.
  - There are no passwords: Hearth keeps a sign-in token in the Windows credential store. There is no tracking,
    no analytics and no ads.
</details>

<p align="center"><sub>Made by <a href="https://github.com/tsumilo">tsumilo</a>, for friends.</sub></p>
