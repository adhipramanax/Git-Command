1. Git clone
   Git clone adalah perintah untuk mengunduh kode sumber yang ada dari repositori jarak jauh (seperti Github, misalnya). Dengan kata lain, Git clone pada dasarnya membuat salinan identik dari versi terbaru proyek dalam repositori dan menyimpannya ke komputer Anda.

   > > : git clone <https://name-of-the-repository-link>

2. Status Git
   Perintah status Git memberi kita semua informasi yang diperlukan tentang cabang saat ini.

   > > : git status

3. Git tambahkan
   Saat kita membuat, memodifikasi, atau menghapus file, perubahan ini akan terjadi di lokal kita dan tidak akan disertakan dalam komit berikutnya (kecuali jika kita mengubah konfigurasi).

- Untuk menambahkan satu file:
  > > : git add <file>
- Untuk menambahkan semuanya sekaligus:
  > > : git add -A / >> : git add .

4. Git Commit
   Ini mungkin perintah Git yang paling sering digunakan. Setelah kami mencapai titik tertentu dalam pengembangan, kami ingin menyimpan perubahan kami (mungkin setelah tugas atau masalah tertentu).

   > > : git commit -m "commit message"

5. Git push
   Setelah melakukan perubahan Anda, hal berikutnya yang ingin Anda lakukan adalah mengirim perubahan Anda ke server jauh. Git Push mengunggah komit Anda ke repositori jarak jauh.

   > > : git push <remote> <branch-name>
   > > Namun, jika cabang Anda baru dibuat, Anda juga perlu mengunggah cabang dengan perintah berikut:
   > > : git push --set-upstream <remote> <name-of-your-branch> / >> :git push -u origin <branch_name>

6. Git Pull
   Perintah git pull digunakan untuk mendapatkan pembaruan dari repo jarak jauh. Perintah ini adalah kombinasi dari git fetch dan git merge yang berarti bahwa, ketika kita menggunakan git pull, ia mendapatkan pembaruan dari repositori jarak jauh (git fetch) dan segera menerapkan perubahan terbaru di lokal Anda (git merge).

   > > : git pull <remote> / >> : git pull

7. Git revert
   Terkadang kita perlu membatalkan perubahan yang telah kita buat. Ada berbagai cara untuk membatalkan perubahan kita secara lokal atau jarak jauh (tergantung pada apa yang kita butuhkan), tetapi kita harus hati-hati menggunakan perintah ini untuk menghindari penghapusan yang tidak diinginkan.

   > > : git revert <code revert>

Quick setup — Git Hub
…or create a new repository on the command line
echo "# Git-Command" >> README.md

> > : git init
> > : git add README.md
> > : git commit -m "first commit"
> > : git branch -M main
> > : git remote add origin <https://name-of-the-repository-link>
> > : git push -u origin main

…or push an existing repository from the command line

> > : git remote add origin <https://name-of-the-repository-link>
> > : git branch -M main
> > : git push -u origin main

…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
