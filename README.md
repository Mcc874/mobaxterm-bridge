# mobaxterm-bridge

mobaxterm-bridge 是一个 MobaXterm 终端桥接skill，让 AI 能直接读写 MobaXterm 终端，无需人工复制粘贴。 核心机制：自动识别当前打开的终端窗口（串口，ssh等），自动搜索日志文件位置，通过读日志获取终端输出，通过 pywinauto send_keys 发送命令，实现 AI 与终端的双向通信。 实现 Linux 开发板、终端等设备的便携式自动化运维——AI 在本地运行即可远程驱动开发板，无需将 AI 部署到目标板上。省去交叉编译、模型移植、运行时部署的繁琐流程,免去环境搭建与反复调试，让嵌入式设备便携实现 AI 自动化能力。 适用场景：嵌入式开发板的串口控制与调试、ssh终端远程自动化、需要 AI 直接驱动终端的自动化任务。

mobaxterm-bridge is a MobaXterm terminal bridging skill that enables AI to read from and write to MobaXterm terminals directly, eliminating manual copy-paste.
Core mechanism: It automatically identifies the currently open terminal window (serial, SSH, etc.), auto-discovers log file locations, retrieves terminal output by reading logs, and sends commands via pywinauto send_keys, achieving bidirectional communication between AI and the terminal.It enables portable automated operations for Linux development boards, terminals, and other devices — AI runs locally while remotely driving the development board, with no need to deploy AI onto the target device. This eliminates the tedious processes of cross-compilation, model porting, and runtime deployment, bypasses environment setup and repeated debugging, and brings AI automation capabilities to embedded devices in a portable way.Use cases: serial control and debugging of embedded development boards, SSH terminal remote automation, and any automation task that requires AI to drive a terminal directly.



mabaxterms设置
<img width="1445" height="981" alt="image" src="https://github.com/user-attachments/assets/503c35c9-ff7b-4369-80a3-bd1e3930747f" />

如果不输出.log或.log不被更改可右键对应的session查看是否被更改，没有则勾选
<img width="1412" height="853" alt="image" src="https://github.com/user-attachments/assets/bab0080d-4607-4317-bc7d-8a5615613d25" />

<img width="1272" height="844" alt="image" src="https://github.com/user-attachments/assets/876a27fc-3549-4e6f-b6fd-1b32bb213f09" />

skill安装完成后 输入 “moba启动” 就可以启动skill
<img width="1503" height="658" alt="image" src="https://github.com/user-attachments/assets/e4c54702-e82c-43d3-939a-93b82697047f" />



输入要求便可以自动输入代码，并自行查看终端状态
<img width="1551" height="368" alt="image" src="https://github.com/user-attachments/assets/c697ab34-9291-4f2c-a1b4-6d29a093fa88" />
<img width="1763" height="1170" alt="image" src="https://github.com/user-attachments/assets/5715eafb-44fd-4423-b611-dba6b8d433a6" />



最终成品
<img width="1597" height="1002" alt="image" src="https://github.com/user-attachments/assets/ac7ac500-8a06-4e8e-bf9b-8136217daa0a" />


注：如果skill不能识别请检查.log是否生成(可直接告诉ai .log 的位置)
<img width="1090" height="656" alt="image" src="https://github.com/user-attachments/assets/18f29850-235c-442e-926e-ca6ac80a9756" />


