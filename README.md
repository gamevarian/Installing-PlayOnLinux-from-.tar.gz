<h1>🖥️ Installing PlayOnLinux from .tar.gz (v4.3.4)</h1>

<h2>🛠 Prerequisites</h2>
<p>Before starting, make sure your system has the following dependencies installed:</p>
<ul>
  <li>Python (version 2.x or 3.x)</li>
  <li>Wine (Windows compatibility layer)</li>
  <li>Xterm (a lightweight terminal emulator)</li>
  <li>Unzip, Wget (for downloading and extracting files)</li>
</ul>
<p>Install them using:</p>
<pre><code>sudo apt update
sudo apt install python3 wine xterm unzip wget</code></pre>
<p><strong>💡 Tip:</strong> If you're using a non-Debian-based distro (like Fedora or Arch), replace <code>apt</code> with your distro's package manager (e.g., <code>dnf</code>, <code>pacman</code>).</p>

<h2>📦 Step 1: Download the .tar.gz File</h2>
<p>Download PlayOnLinux version 4.3.4:</p>
<pre><code>wget https://www.playonlinux.com/script_files/PlayOnLinux/4.3.4/PlayOnLinux_4.3.4.tar.gz</code></pre>

<h2>📂 Step 2: Extract the Archive</h2>
<p>Extract the downloaded archive:</p>
<pre><code>tar -xvzf PlayOnLinux_4.3.4.tar.gz</code></pre>

<h2>🚀 Step 3: Run PlayOnLinux</h2>
<p>Navigate to the extracted folder and run the program:</p>
<pre><code>cd PlayOnLinux/
./playonlinux</code></pre>
<p>If it doesn't run due to permission issues, add execute permissions:</p>
<pre><code>chmod +x playonlinux
./playonlinux</code></pre>

<h2>🧪 Optional: Create a Desktop Shortcut</h2>
<p>Create a launcher to access PlayOnLinux from your app menu:</p>
<pre><code>nano ~/.local/share/applications/playonlinux.desktop</code></pre>
<p>Paste the following configuration (update paths to match your system):</p>
<pre><code>[Desktop Entry]
Name=PlayOnLinux
Exec=/path/to/PlayOnLinux/playonlinux
Type=Application
Categories=Utility;
Icon=/path/to/PlayOnLinux/etc/playonlinux.png</code></pre>
<p><strong>🔐 Note:</strong> Make sure the <code>Icon</code> path points to a valid PNG file. You can use any icon you prefer.</p>

<h2>❓ Troubleshooting</h2>
<ul>
  <li><strong>Wine not working?</strong> Run <code>winecfg</code> to initialize Wine and check for errors.</li>
  <li><strong>Missing dependencies?</strong> Check terminal messages and install any packages mentioned.</li>
  <li><strong>Still can’t launch?</strong> Try running with <code>python3 playonlinux</code> explicitly.</li>
</ul>

<h2>📌 Additional Notes</h2>
<ul>
  <li>PlayOnLinux creates isolated Wine prefixes per application.</li>
  <li>Advanced settings like Wine version management are available after launching.</li>
  <li>For gaming, ensure your graphics drivers are up to date.</li>
</ul>

<p><strong>📚 Source:</strong> <a href="https://www.gamevarian.com/2025/07/panduan-software-game-windows-di-linux.html" target="_blank">Gamevarian – Guide to Running Windows Games on Linux (2025)</a></p>
