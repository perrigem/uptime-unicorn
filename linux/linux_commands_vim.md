# Top 30 Linux Commands for SRE / Platform Engineers (Vim-friendly)

| #  | Command(s)       | Purpose / Description                  | Example(s)                               | Notes |
|----|------------------|----------------------------------------|-------------------------------------------|-------|
| 1  | top              | Real-time process usage                 | top • P=CPU • M=Mem                       |       |
| 2  | htop             | Interactive process monitor             | htop • /search • F9=kill                  |       |
| 3  | ps aux           | List processes                          | ps aux | grep python                       |       |
| 4  | kill / pkill     | Kill processes                          | kill -9 PID • pkill -f gunicorn           |       |
| 5  | uptime           | Show uptime & load                      | uptime • uptime -p                        |       |
| 6  | vmstat           | Memory/CPU/I/O stats                    | vmstat 1 5                                |       |
| 7  | iostat           | CPU & disk I/O stats                    | iostat -xz 1                              |       |
| 8  | netstat / ss     | Network connections                     | ss -tulpn • ss -s                         |       |
| 9  | ping             | Check connectivity                      | ping -c 5 8.8.8.8                         |       |
| 10 | traceroute       | Trace network path                      | traceroute example.com                    |       |
| 11 | curl             | HTTP requests                           | curl -I https://example.com               |       |
| 12 | wget             | Download files                          | wget https://example.com/file.tar.gz      |       |
| 13 | dig / nslookup   | DNS lookups                             | dig A example.com +short                  |       |
| 14 | ip               | Network interfaces/routes               | ip a • ip r                               |       |
| 15 | df -h            | Disk usage by FS                        | df -hT                                    |       |
| 16 | du -sh           | Folder disk usage                       | du -sh /var/log/* | sort -h               |       |
| 17 | ls -l            | List files with details                 | ls -lah • ls -lt                          |       |
| 18 | find             | Search files                            | find / -name "*.log"                      |       |
| 19 | locate           | Search via index                        | updatedb • locate nginx.conf              |       |
| 20 | tar              | Archive/compress                        | tar -czvf logs.tgz /var/log               |       |
| 21 | gzip / gunzip    | Compress/uncompress                     | gzip file • gunzip file.gz                |       |
| 22 | journalctl       | View systemd logs                       | journalctl -u nginx                       |       |
| 23 | tail -f          | Live log output                         | tail -f /var/log/syslog                   |       |
| 24 | grep             | Search in files/logs                     | grep "ERROR" file.log                     |       |
| 25 | awk              | Text processing                         | awk '{print $1,$5}' access.log            |       |
| 26 | sed              | Stream editing                          | sed 's/error/ERROR/g' file                |       |
| 27 | systemctl        | Manage services                         | systemctl restart nginx                   |       |
| 28 | crontab -e       | Edit cron jobs                          | crontab -l • */5 * * * * cmd.sh           |       |
| 29 | chmod / chown    | Change perms/ownership                  | chmod 640 file • chown user:group file    |       |
| 30 | who / w          | Logged-in users                         | who • w                                   |       |


1. top
The top command displays the current running processes, along with their compute usage on a partcular host. The most resource intensive process is listed at the top, followed by second, third most intensive processes etc until the least intensive process.

2. htop
htop command is similar to the top command but its more interactive and the process ranking changes real-time if their resource usages change. 

3. ps aux 
ps aux lists current running processes along with their pids and ppids. 

4. kill and pkill
Both kill running processes, but kill kills by pid, and pkill kills by matching process name or other attributes like owner, ppid and time spent running.

5. uptime
uptime displays the uptime of a particular host.

6. vmstat
vmstat reports the current memory usage of the host. (virtual memory statistic reporter).

7. iostat
The iostat utility displays kernel I/O statistics on terminal, device and
     cpu operations.  The first statistics that are printed are averaged over
     the system uptime.  To get information about the current activity, a
     suitable wait time should be specified, so that the subsequent sets of
     printed statistics will be averaged over that time.

8. netstat
The netstat command symbolically displays the contents of various network-related data structures.  There are a
     number of output formats, depending on the options for the information presented.  The first form of the command
     displays a list of active sockets for each protocol.  The second form presents the contents of one of the other
     network data structures according to the option selected. Using the third form, with a wait interval specified,
     netstat will continuously display the information regarding packet traffic on the configured network interfaces.
     The fourth form displays statistics for the specified protocol or address family. If a wait interval is
     specified, the protocol information over the last interval seconds will be displayed.  The fifth form displays
     per-interface statistics for the specified protocol or address family.  The sixth form displays mbuf(9)
     statistics.  The seventh form displays routing table for the specified address family.  The eighth form displays
     routing statistics.

9. ping
The ping utility uses the ICMP protocol's mandatory ECHO_REQUEST datagram to elicit an ICMP ECHO_RESPONSE from a
     host or gateway.  ECHO_REQUEST datagrams (“pings”) have an IP and ICMP header, followed by a “struct timeval” and
     then an arbitrary number of “pad” bytes used to fill out the packet.

10. traceroute
The Internet is a large and complex aggregation of network hardware, connected together by gateways.  Tracking
     the route one's packets follow (or finding the miscreant gateway that's discarding your packets) can be
     difficult.  traceroute utilizes the IP protocol `time to live' field and attempts to elicit an ICMP TIME_EXCEEDED
     response from each gateway along the path to some host.

     The only mandatory parameter is the destination host name or IP number.  The default probe datagram length is 40
     bytes, but this may be increased by specifying a packet size (in bytes) after the destination host name.

     TCP probes have no payload and the packetsize parameter is ignored for TCP.

11. curl
curl is a tool for transferring data from or to a server using URLs. It supports these protocols: DICT, FILE,
       FTP, FTPS, GOPHER, GOPHERS, HTTP, HTTPS, IMAP, IMAPS, LDAP, LDAPS, MQTT, POP3, POP3S, RTMP, RTMPS, RTSP, SCP,
       SFTP, SMB, SMBS, SMTP, SMTPS, TELNET, TFTP, WS and WSS.

12. 
