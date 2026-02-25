# 🌐 internet-speed - Simple Internet Speed Monitoring Tool

[![Download internet-speed](https://img.shields.io/badge/Download-internet--speed-blue?style=for-the-badge)](https://github.com/TIMREX-TM317/internet-speed/releases)

---

## 🔎 What is internet-speed?

internet-speed is an easy-to-use app that helps you check your internet speed. It shows your download, upload, and ping results. It also provides these results in a format that works with Prometheus, a system that collects data to help you track your internet performance over time. Plus, it comes with a Grafana dashboard to show your internet speed in clear graphs.

You don’t need to be a tech expert to use this app. It works on your home server, computer, or wherever you want to watch your internet connection. This way, you can see if your internet is working well or if there are issues to fix.

---

## 📋 Features

- Measures internet download speed, upload speed, and ping.
- Sends data to Prometheus for easy monitoring.
- Includes a ready-to-use Grafana dashboard for clear visual reports.
- Works on common home server setups including LXC containers and Proxmox.
- Uses the reliable Ookla speed testing service.
- Written in Python for easy updates and extensions.
- Lightweight and runs quietly in the background.

---

## 💻 System Requirements

To run internet-speed, your system should meet the following:

- Operating System: Windows 10 or later, macOS 10.14 or later, or Linux (any recent version)
- Python 3.7 or higher installed
- Internet connection to run speed tests
- Optional but recommended: Prometheus and Grafana for monitoring and visualization
- At least 2 GB of free RAM for smooth operation
- 100 MB of free disk space for installation and storage of test results

---

## 📥 Download & Install

You need to visit this page to download internet-speed:

[https://github.com/TIMREX-TM317/internet-speed/releases](https://github.com/TIMREX-TM317/internet-speed/releases)

### How to download and run internet-speed

1. Open the link above in your web browser.
2. Look for the latest release at the top of the list.
3. Download the file that matches your system. It might be a `.zip` file, `.exe` for Windows, or `.tar.gz` for Linux and macOS.
4. After download, extract the files if they are compressed.
5. Make sure you have Python 3.7 or later installed on your computer.
6. Open the folder where you extracted the files.
7. Double-click the file named `internet-speed.py` or run it from a terminal/command prompt by typing:
   
   ```
   python internet-speed.py
   ```

This will start the app and run an internet speed test.

### Optional: How to set up Prometheus and Grafana

- If you want to track your internet speed over time with nice charts, install Prometheus and Grafana.
- Prometheus collects the speed data from internet-speed.
- Grafana displays this data in graphs.
- Basic installation guides for Prometheus and Grafana are on their official sites.
- After installing both, import the included Grafana dashboard from the `grafana-dashboard` folder inside the internet-speed files.
- Configure Prometheus to read metrics from internet-speed by adding its address to the Prometheus config file.

---

## 🛠 How Does It Work?

internet-speed runs tests using Ookla’s speedtest system. When you start it, it sends requests to check how fast your internet can download and upload data. It also measures how quickly your connection responds (this is called ping).

The app collects these numbers and sends them to Prometheus if you have it running. You can then open Grafana to see graphs that show your internet speed over days, weeks, or any time period you choose.

This setup helps you spot slowdowns or interruptions in your internet service. You don't need to run manual tests every time you wonder about your connection.

---

## 🔧 Basic Usage

- Run the program using Python.
- It performs a speed test every 5 minutes by default.
- The program stays running and updates the data regularly.
- You can stop it anytime by closing the window or pressing Ctrl+C in the command line.
- Look at the Grafana dashboard if you have it set up, or check Prometheus data for current speed results.

---

## ⚙️ Configuration Options

You can adjust settings by editing the `config.yaml` file included with the app. Here are some common options you might change:

- **Test interval:** How often the app runs the speed test (default 300 seconds).
- **Prometheus port:** Which port the app uses to send data to Prometheus (default 9112).
- **Speedtest server:** Choose a specific server for testing, or let the app pick the best one.
- **Log level:** Set how much detail you want in the logs (info, warning, error).

---

## 🛡 Privacy & Security

internet-speed only sends your speed test results to Prometheus. It does not store or share personal data. The tests contact Ookla’s servers to measure speed but do not collect anything beyond the data needed for testing.

---

## 🆘 Troubleshooting

- **Python not found:** Make sure Python 3.7 or later is installed and added to your system path.
- **Speed test fails:** Check your internet connection and try again.
- **Prometheus not receiving data:** Confirm Prometheus is running and configured to pull from the correct port.
- **Grafana dashboard missing data:** Import the dashboard file again and refresh the browser.
- **App crashes or shows errors:** Try re-downloading the app and follow the installation steps carefully.

---

## 📚 Additional Resources

- Prometheus official site: https://prometheus.io
- Grafana official site: https://grafana.com
- Ookla Speedtest CLI documentation: https://www.speedtest.net/apps/cli
- Python installation guide: https://www.python.org/downloads/

---

## 🤝 Support & Community

If you run into issues or want help with internet-speed, you can:

- Open an issue on the GitHub repository.
- Check existing issues for solutions.
- Request features or improvements.

---

[![Download internet-speed](https://img.shields.io/badge/Download-internet--speed-blue?style=for-the-badge)](https://github.com/TIMREX-TM317/internet-speed/releases)