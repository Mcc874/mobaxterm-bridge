# mobaxterm-bridge
修正：目前mobaxterm只能输出串口log
Correction: MobaXterm can only output serial port logs

mobaxterm-bridge 是一个 MobaXterm 终端桥接skill，让 AI 能直接读写 MobaXterm 终端，无需人工复制粘贴。 核心机制：自动识别当前打开的终端窗口（串口），自动搜索日志文件位置，通过读日志获取终端输出，通过 pywinauto send_keys 发送命令，实现 AI 与终端的双向通信。 实现 Linux 开发板、终端等设备的便携式自动化运维——AI 在本地运行即可远程驱动开发板，无需将 AI 部署到目标板上。省去交叉编译、模型移植、运行时部署的繁琐流程,免去环境搭建与反复调试，让嵌入式设备便携实现 AI 自动化能力。 适用场景：嵌入式开发板的串口控制与调试、需要 AI 直接驱动终端的自动化任务。

mobaxterm-bridge is a MobaXterm terminal bridging tool that lets AI directly read from and write to MobaXterm terminals, eliminating manual copy-paste.
Core mechanism: it auto-detects the currently open terminal window (works for serial), auto-discovers the log file location, reads terminal output by tailing the log, and injects commands via pywinauto send_keys — enabling full bidirectional AI↔terminal communication.
Core value: enables portable, automated operation of Linux dev boards, terminals and similar devices — the AI runs locally and drives the board remotely, with no need to deploy the AI onto the target board. This dramatically cuts operational cost (no cross-compiling, model porting, or runtime deployment), time cost (skip environment setup and repeated debugging), and technical cost (resource-constrained boards can't easily run inference locally — the bridge sidesteps the hardware barrier entirely, bringing AI automation to embedded devices regardless of their compute limits).
Use cases: serial-console control and debugging of embedded dev boards, any automation where AI must drive a terminal directly.



mabaxterms设置
<img width="1445" height="981" alt="image" src="https://github.com/user-attachments/assets/503c35c9-ff7b-4369-80a3-bd1e3930747f" />



skill安装完成后 输入 “moba启动” 就可以启动skill
<img width="1503" height="658" alt="image" src="https://github.com/user-attachments/assets/e4c54702-e82c-43d3-939a-93b82697047f" />



输入要求便可以自动输入代码，并自行查看终端状态
<img width="1551" height="368" alt="image" src="https://github.com/user-attachments/assets/c697ab34-9291-4f2c-a1b4-6d29a093fa88" />
<img width="1763" height="1170" alt="image" src="https://github.com/user-attachments/assets/5715eafb-44fd-4423-b611-dba6b8d433a6" />



最终成品
<img width="1597" height="1002" alt="image" src="https://github.com/user-attachments/assets/ac7ac500-8a06-4e8e-bf9b-8136217daa0a" />


注：如果skill不能识别请检查.log是否生成(可直接告诉ai .log 的位置)
<img width="1090" height="656" alt="image" src="https://github.com/user-attachments/assets/18f29850-235c-442e-926e-ca6ac80a9756" />


