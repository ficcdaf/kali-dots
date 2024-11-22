# kali-dots

My Kali Linux dotfiles. Optimized to run well in a VM.

I run Kali on an Arch Linux host inside VirtualBox. I installed the `kali-i3` ISO, but there were some serious issues with the graphics rendering. The default picom settings, while looking good, are way too heavy with all the transparency and blur. Kitty is also not a good choice for a terminal in a VM with GPU acceleration disabled (which is necessary sadly, otherwise the VM actually freaks out).

These dots are basically the default Kali i3 dotfiles from the Kali repository, with my own modifications and some of my dotfiles from my main machine. I don't sync them directly from Kali because I definitely don't want my GitHub private key on my attack box.

Some considerations: ZelliJ is not available in the Kali package repo, and its version of Neovim is too old for my configuration, so you will need to download the tarballs manually. This Neovim config also needs npm and cargo which are not installed by default on Kali.
