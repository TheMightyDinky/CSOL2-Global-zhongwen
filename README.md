# CSOL2-Global-中文 (CN LOCALISATION FILES FOR CSOL2 GLOBAL)
# 许可协议 (LICENSE)
This localization project is not affiliated with Valve or Nexon. It's for use with "Counter-Strike: Online 2 Global" only. CSO2 is owned by Nexon and Valve. Any remix or derivative of this project must be shared under the same license. Licensed under Creative Commons Attribution-ShareAlike 4.0.

本地化项目与 Valve 公司 或 Nexon 公司 无任何隶属或合作关系，仅用于 《反恐精英OL2》（全球服）。《反恐精英OL2》 的版权及所有相关权利归 Nexon 公司 与 Valve 公司共同所有。任何基于该游戏的修改行为，均须遵循此许可协议。
本作品采用知识共享署名-相同方式共享4.0版国际许可协议授权。

# 关于本模组（About the mod）
Made by TheMightyDinky. Code adapted from CSO2 QingXue, fixed and compiled by TheMightyDinky. Translation help from TeardropWaltz.
模组由 THE MIGHTY DINKY 制作，代码由"CSO2 晴雪服"提供，由 THE MIGHTY DINKY 编译修复，由玩家 TeardropWaltz 提供翻译文本。

# What's included: 
New lobby promo banner, CN font, Chinese bot voicelines, Chinese tutorial voicelines, ime.xml file, an improved QingXue bot profile (worth considering as the new default, in my opinion), modified Simplified Chinese files from CSOL2 (QingXue/QQ), and a bad-word censor script (untested on Global, may or may not work).

# 安装模组指南（Guide for installing the mod)
Link: https://drive.google.com/file/d/1Frsf6xsx8J1mO_Qa9VZFoquuwtR0yCxB/view
Youtube: https://www.youtube.com/watch?v=Ai_8mu9RdpI

# Why this exists:
The Chinese CSO2 community didn't have a clean, vanilla-compatible Chinese localization for the Global client — only the heavily modified private-server builds like QingXue. So I pulled the localization files out of QingXue's build to create a proper Chinese language option for Global.
The problem: QingXue's files were stripped-down and missing entries for weapons, items, and characters that only exist in Global. Running the game with just those files caused new items to show up as raw internal filenames instead of proper names.

# How I fixed it:
Cross-referenced the vanilla English files and manually added the missing entries into the Chinese files, so new Global items display correctly.
Playtested repeatedly to catch text/UI issues; menu rendering, clipping, font display.
Used launch parameters (-decryptedfiles, -enablecustom) to get around the engine's encrypted file-path restrictions, so custom fonts, bot profiles, the censor script, and audio files would load properly.
Brought in TeardropWaltz, a native Chinese speaker, to help translate and check high-volume text; game modes, weapon names, trophies, and documentation.

-ZH- 玩家需把模组文件下的整个文件夹与在CSO2目录下的对应文件夹进行整体替换（CSO2目录下需替换的文件大多位于D:\CSO2\Data\cstrike下,或D:\CSO2处的custom）
玩家需要将所需复制的具体文件夹，如模组中的sound文件夹复制到对应的CSO2文件下的sound处，并在系统提示是否覆盖时选择"覆盖全部"（每个文件都这么处理）请勿直接将模组中的某个大文件夹直接丢到CSO2中，这样游戏文件下的英文文件并未得到替换因而无法有效运行
最后, 玩家打开游戏客户端, 点击位于"Launch"登录下面的"setting"设置, 点击英文"override", 然后将以下命令复制到空行上：
-lang schinese -masterip global -masterport 30001 -decryptedfiles -enablecustom -debugconsole -debuginfo -username [?] -password [?]
username指用户名, password指密码 (注意：不要删除原本空格和符号-, [?]处填写个人在游戏官网注册的账号和密码)
例如: -lang schinese -masterip global -masterport 30001 -decryptedfiles -enablecustom -debugconsole -debuginfo -username cat -password 1234
操作完成后右上角x掉弹窗,开启游戏,游戏语言就改好了.

-EN- Replace your game files with the ones from the mod folder, matching them to the corresponding folders in your CSO2 directory (most files go in D:\CSO2\Data\cstrike, or custom under D:\CSO2).
Example: copy the mod's sound folder contents into CSO2's sound folder, choosing "overwrite all" when prompted (do this for each folder). Don't drag whole folders from the mod straight into CSO2 — that replaces the folder itself instead of merging the files inside it, and the game won't work correctly.
Then open the game client, go to Settings under "Launch," click "override," and paste in this command:
-lang schinese -masterip global -masterport 30001 -decryptedfiles -enablecustom -debugconsole -debuginfo -username [?] -password [?]
(username/password are your account login — don't delete the spaces or dashes)
Example: -lang schinese -masterip global -masterport 30001 -decryptedfiles -enablecustom -debugconsole -debuginfo -username cat -password 1234
Close the popup in the top-right corner, launch the game, and the language will be changed.
