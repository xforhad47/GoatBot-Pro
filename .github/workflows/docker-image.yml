module.exports = {
  config: {
    name: "commandname",
    version: "1.0.0",
    author: "YourName",
    countDown: 5,
    role: 0,
    shortDescription: "...",
    longDescription: "...",
    category: "fun",
    guide: "{prefix}commandname [args]"
  },

  onStart: async function ({ api, event, args, message, getLang }) {
    message.reply("Hello!");
  },

  onReply: async function ({ api, event, Reply, message }) {
    if (event.senderID !== Reply.author) return;
    message.reply(`You replied: ${event.body}`);
  },

  onReaction: async function ({ api, event, Reaction, message }) {
    message.reply(`You reacted with: ${event.reaction}`);
  },

  onChat: async function ({ api, event, message }) {
    if (event.body === "hello") message.reply("hi!");
  },

  onEvent: async function ({ api, event, message }) {
    if (event.logMessageType === "log:subscribe") {
      message.reply("Welcome!");
    }
  }
};
