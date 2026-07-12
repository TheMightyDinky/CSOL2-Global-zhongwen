# CSOL2-Global-中文 (CN LOCALISATION FILES FOR CSOL2 GLOBAL)
# 许可协议 (LICENSE)
This localisation Project is not affiliated with either Valve or Nexon, and is to be used only for "Counter-Strike: Online 2 Global".
Counter-Strike: Online 2 is owned by both Nexon and Valve. Remixing, building upon this material, or transforming it requires that you distribute your contributions under the same license as the one used for my project. This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 Unported License.

本地化项目与 Valve 公司 或 Nexon 公司 无任何隶属或合作关系，仅用于 《反恐精英OL2》（全球服）。《反恐精英OL2》 的版权及所有相关权利归 Nexon 公司 与 Valve 公司共同所有。任何基于该游戏的修改行为，均须遵循此许可协议。
本作品采用知识共享署名-相同方式共享4.0版国际许可协议授权。

# 关于本模组（About the mod）
模组由 THE MIGHTY DINKY 制作（MOD CREATED BY THEMIGHTYDINKY）
代码由“CSO2 晴雪服”提供, 由THE MIGHTY DINKY 编译修复（CODE BORROWED FROM CSO2 QINGXUE, EDITED AND FIXED BY THEMIGHTYDINKY）
由玩家TeardropWaltz提供翻译文本（HELPED WITH THE TRANSLATION BY TEARDROPWALTZ）

This pack contains: New lobby promotion banner, CN_font, Chinese voicelines for bots, Tutorial Chinese voicelines, ime.xml file, QingXue Botprofile (Better than the current one in my opinion; I would actually suggest this botprofile to Organner so we could replace the old one), Modification of the Simplified Chinese files from CSOL2 (aka CSO2 QingXue, CSO2 QQ), Bad word censor script (Might work on Global; not tested)

# 安装模组指南（Guide for installing the mod)
Link: https://drive.google.com/file/d/1Frsf6xsx8J1mO_Qa9VZFoquuwtR0yCxB/view
Youtube: https://www.youtube.com/watch?v=Ai_8mu9RdpI

### Architecture & Technical Implementation

#### 1. Problem Statement & System Discrepancies
The Chinese CSOL2 Community lacked a vanilla-compatible localization file for the *CSO2 Global* launcher/Game, restricting players to play on the highly modified, asset-bloated private server clients of CSOL2 (such as *QingXue*). In order to create a clean, vanilla Simplified Chinese language environment on the global executable, the localization files were extracted from the QingXue server build. However, this database was severely stripped-down and lacked the mandatory configuration strings for weapons, assets, and character models newly introduced to the *CSO2 Global* version.

#### 2. String Migration, Data Validation & UI Patching
Because the QingXue Chinese files lacked structural alignment with the Global build, running the game caused critical text asset failures, where newly added weapons and character items would display broken, raw internal system filenames instead of their correct, user-facing titles. System execution passes included:
*   **Database Synchronization:** Cross-referenced and extracted structural database parameters from the vanilla English localization logs, manually injecting the missing configuration lines into the Chinese language dictionary to map proper text titles onto global items.
*   **UI Hierarchy Testing & Layout Verification:** Conducted extensive runtime validation and game playtesting frames to ensure text boxes, user-interface menus, and font layout layers displayed strings correctly without client-side asset clipping or menu-rendering bugs.
*   **Decryption & Command Routing:** Configured command-line parameters (`-decryptedfiles`, `-enablecustom`) to force the engine client to bypass default encrypted pak file path limits, successfully routing the game runtime to read custom typographical fonts, bot profiles, bad-word filter scripts, and audio telemetry files natively.

#### 3. Collaborative Development Loops
To manage individual language limits while keeping peak velocity on testing UI stability and fixing command-line launcher compatibility, translation strings were crowd-sourced. A native Chinese partner (`TeardropWaltz`) was brought into the pipeline to translate and audit high-density text files for game modes, specialized weapons, trophies, and localized documentation.

-ZH-
玩家需把模组文件下的整个文件夹与在CSO2目录下的对应文件夹进行整体替换（CSO2目录下需替换的文件大多位于D:\CSO2\Data\cstrike下,或D:\CSO2处的custom）

玩家需要将所需复制的具体文件夹，如模组中的sound文件夹复制到对应的CSO2文件下的sound处，并在系统提示是否覆盖时选择“覆盖全部”（每个文件都这么处理）请勿直接将模组中的某个大文件夹直接丢到CSO2中，这样游戏文件下的英文文件并未得到替换因而无法有效运行

最后, 玩家打开游戏客户端, 点击位于“Launch”登录下面的“setting”设置, 点击英文“override”, 然后将以下命令：-lang schinese -masterip global -masterport 30001 -decryptedfiles -enablecustom -debugconsole -debuginfo -username [?] -password [?] 复制到空行上, username指用户名, password指密码 (注意： 不要删除原本空格和符号-, [?]处填写个人在游戏官网注册的账号和密码)
例如: -lang schinese -masterip global -masterport 30001 -decryptedfiles -enablecustom -debugconsole -debuginfo -username cat -password 1234
操作完成后右上角x掉弹窗,开启游戏,游戏语言就改好了.


-EN-
Players need to replace the game's files with the ones from the mod's folders; the change should take place at the corresponding folders in the CSO2 directory (most of the files that need to be replaced in the CSO2 directory are located at D:\CSO2\Data\cstrike, or custom at D:\CSO2)

E.g: Players need to bring the specific files within the mod's folders, such as the sound files, to the sound folder under the corresponding CSO2 game directory (this is done for each file). Do not directly drop the respective folders from the mod into CSO2's directory, otherwise the game's folders will be replaced and not the files within them.

Now, the player should open the game client, click the settings under the "Launch" button, clicks the "override" text, and then copy the following command and paste it into that box: -lang schinese -masterip global -masterport 30001 -decryptedfiles -enablecustom -debugconsole -debuginfo -username [?] -password [?] to a blank line, username refers to the user name, password refers to the password (Note: Do not delete the original spaces and "-" symbols; Now fill these "[?]" with the account and password registered on the game's official website)

E.g: -lang schinese -masterip global -masterport 30001 -decryptedfiles -enablecustom -debugconsole -debuginfo -username cat -password 1234
After the operation is completed, remove the pop-up window in the upper right corner, open the game, and the game language will be changed.
