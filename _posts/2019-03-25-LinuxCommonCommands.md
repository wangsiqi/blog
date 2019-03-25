---
layout:     post
title:      Linux 常用命令
subtitle:   摘抄Linux常用命令
date:       2019-03-25 16:28:26 +0800
author:     wangsiqi
header-img: img/post-bg-github-cup.jpg
catalog: true
tags:                              
    - Linux
---
# 操作文件目录

<html>
    <table style="width:100%" >
        <thead>
            <tr>
                <th>命令</th>
                <th>说明</th>
                <th>语法</th>
                <th>参数</th>
                <th>参数说明</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>cd</td>
                <td>切换目录</td>
                <td>cd [dirName]</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td rowspan="2">ls</td>
                <td rowspan="2">显示文件和目录列表</td>
                <td rowspan="2">ls [-alrtAFR] [name…]</td>
                <td>-l</td>
                <td>列出文件的详细信息</td>
            </tr>
            <tr>
                <td>-a</td>
                <td>列出当前目录所有文件，包含隐藏文件</td>
            </tr>
            <tr>
                <td>mkdir</td>
                <td>创建目录</td>
                <td>mkdir [-p] dirName</td>
                <td>-p</td>
                <td>父目录不存在情况下先生成父目录</td>
            </tr>
            <tr>
                <td>touch</td>
                <td>创建文件</td>
                <td>touch [fileName]</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td rowspan="3">echo</td>
                <td>控制台输出内容</td>
                <td>echo hello</td>
                <td></td>
                <td></td>
            </tr>       
            <tr>
                <td>内容追加到文件</td>
                <td>echo hello > t.txt</td>
                <td></td>
                <td></td>
            </tr>  
            <tr>
                <td>内容覆盖文件内容</td>
                <td>echo hello >> t.txt</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>cat</td>
                <td>显示文本文件内容</td>
                <td>cat [-AbeEnstTuv] [–help] [–version] fileName</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>cp</td>
                <td>复制文件或目录</td>
                <td>cp [options] source dest</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td rowspan="2">rm</td>
                <td rowspan="2">删除文件</td>
                <td rowspan="2">rm [options] name…</td>
                <td>-f</td>
                <td>强制删除文件或目录</td>
            </tr>
            <tr>
                <td>-r</td>
                <td>同时删除该目录下的所有文件</td>
            </tr>
            <tr>
                <td>find</td>
                <td>查找指定的文件</td>
                <td></td>
                <td>-name</td>
                <td>文件名</td>
            </tr>
            <tr>
                <td>grep</td>
                <td>指定的文本文件中查找指定的字符串</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>tree</td>
                <td>用于以树状图列出目录的内容</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>pwd</td>
                <td>显示当前工作目录</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>ln</td>
                <td>建立软链接</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>more</td>
                <td>分页显示文本文件内容</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>head</td>
                <td>显示文件开头内容</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>tail</td>
                <td>显示文件结尾内容</td>
                <td></td>
                <td>-f</td>
                <td>跟踪输出</td>
            </tr>
        </tbody>
    </table>
</html>

# 系统管理命令
<html>
    <table style="width:100%" >
        <thead>
            <tr>
                <th>命令</th>
                <th>说明</th>
                <th>语法</th>
                <th>参数</th>
                <th>参数说明</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td rowspan="10">shutdown</td>
                <td rowspan="10">关机或重启</td>
                <td rowspan="10">shutdown [-t seconds] [-rkhncfF] time [message]</td>
                <td>-t seconds</td>
                <td>设定在几秒钟之后进行关机程序</td>
            </tr>
            <tr>
                <td>-k</td>
                <td>并不会真的关机，只是将警告讯息传送给所有只用者</td>
            </tr>
            <tr>
                <td>-r</td>
                <td>关机后重新开机(重启)</td>
            </tr>
            <tr>
                <td>-h</td>
                <td>关机后停机</td>
            </tr>
            <tr>
                <td>-n</td>
                <td>不采用正常程序来关机，用强迫的方式杀掉所有执行中的程序后自行关机</td>
            </tr>
            <tr>
                <td>-c</td>
                <td>取消目前已经进行中的关机动作</td>
            </tr>
            <tr>
                <td>-f</td>
                <td>关机时，不做 fcsk 动作(检查 Linux 档系统)</td>
            </tr>
            <tr>
                <td>-F</td>
                <td>关机时，强迫进行 fsck 动作</td>
            </tr>
            <tr>
                <td>time</td>
                <td>设定关机的时间</td>
            </tr>
            <tr>
                <td>message</td>
                <td>传送给所有使用者的警告讯息</td>
            </tr>
            <tr>
                <td>reboot</td>
                <td>关机后重新开机(重启)</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>stat</td>
                <td>显示指定文件的相关信息,比ls命令显示内容更多</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>who</td>
                <td>显示在线登录用户</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>hostname</td>
                <td>显示主机名称</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>uname</td>
                <td>显示系统信息</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>top</td>
                <td>显示当前系统中耗费资源最多的进程</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>ps</td>
                <td>显示瞬间的进程状态</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>du</td>
                <td>显示指定的文件（目录）已使用的磁盘空间的总量</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>df</td>
                <td>显示文件系统磁盘空间的使用情况</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>free</td>
                <td>显示当前内存和交换空间的使用情况</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>ifconfig</td>
                <td>显示网络接口信息</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>ping</td>
                <td>测试网络的连通性</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>netstat</td>
                <td>显示网络状态信息</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>clear</td>
                <td>清屏</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>kill</td>
                <td>杀死一个进程</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
        </tbody>
    </table>
</html>
