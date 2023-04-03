const { Client, Events, GatewayIntentBits } = require('discord.js');

const client = new Client({ intents: [GatewayIntentBits.Guilds, GatewayIntentBits.GuildMembers, GatewayIntentBits.MessageContent, GatewayIntentBits.GuildMessages] });

client.once(Events.ClientReady, c => {
    console.log(`Ready! (${c.user.tag})`);
});

client.on(Events.MessageCreate, message => {
    if (message.author.bot) return; 
    if (message.content.includes("ひま")) {
        message.channel.send("暇らしいね");
    }
    
    if (message.content.includes("暇")) {
        message.channel.send("暇らしいね");
    }

    if (message.content.includes("今日は")) {
        message.channel.send("何もしません");
    }

    if (message.content.includes("そくし")) {
        message.channel.send("なに");
    }

    if (message.content.includes("草")) {
        message.channel.send("wwwwww");
    }

    if (message.content.includes("w")) {
        message.channel.send("wwwwww");
    }

    if (message.content.includes("第五募集中")) {
        message.channel.send("@everyone第五しよーぜ");
    }

    if (message.content.includes("第5募集")) {
        message.channel.send("@everyone第五しよーぜ");
    }
    
    if (message.content.includes("第5募集中")) {
        message.channel.send("@everyone第五しよーぜ");
    }

    if (message.content.includes("第５募集中")) {
        message.channel.send("@everyone第五しよーぜ");
    }

    if (message.content.includes("第５募集")) {
        message.channel.send("@everyone第五しよーぜ");
    }

    if (message.content.includes("第五募集")) {
        message.channel.send("@everyone第五しよーぜ");
    }

    if (message.content.includes("しね")) {
        message.channel.send("黙れ");
    }

    if (message.content.includes("そして#")) {
        message.channel.send(" 灰 と な れ ");
    }

    if (message.content.includes("こん")) {
        message.channel.send("ばんわ");
    }

    if (message.content.includes("うざ")) {
        message.channel.send("散れえええええ");
    }

    if (message.content.includes("ないす")) {
        message.channel.send("よくやった！！！");
    }

    if (message.content.includes("ざーこ")) {
        message.channel.send("ざぁ～こ♡ざぁ～こ♡");
    }

    if (message.content.includes("メスガキみたいに喋って")) {
        message.channel.send("どうしよっかな～♡やっちゃおうかな～♡")
    }
    
    if (message.content.includes("メスガキみたいにおねがい")) {
         MessageManager.cannel.reply("くふふっ♡わざわざ年下の小さい女の子にそんなことお願いするんだ～♡なっさけな～い♡");
       
    }
      
});


client.on("ready", () => {
	console.log("BOTの準備ができました。");
});

client.on('ready', message =>{
    console.log('～準備完了～');







client.login("token");
