# In this page I'll use the raw version of checkmk

## Introduction

<p>Checkmk have 3 version, and the good and easy one is the enterprise version. It's need subscribe to used.
In this article I use the raw edition, it's free and open source</p>

## Install Plugin

<p>In raw edition, we only can add plugin using linux cli</p>
<h3>Setup</h3>

1. we need previllage access <pre> sudo su </pre>
2. look name of sites <pre> omd sites </pre>
3. entry sites docker <pre> omd su "sites name" </pre>

<h3> we can use mkp command to manage our plugin</h3>

1. see all mkp commmand <pre> mkp --help </pre>
2. see all plugin that have been added <pre> mkp list </pre>
3. we can add plugin using files we have downloaded <pre> mkp add "you_mkp_file_pwd" </pre>
3. we can see status of our plugin
4. if status is disable, we can enable it using this command <pre> mkp enable "plugin_name" "plugin_version" </pre>
5. we can look at status to check if it's have enable or not <pre> mkp list </pre>
6. we can see detail of package (plugin) using <pre> mkp show "plugin_name" "plugin_version" </pre>
