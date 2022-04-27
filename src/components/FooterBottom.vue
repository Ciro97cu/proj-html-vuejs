<template>
  <div>
    <div class="container-sm pb-5">
      <div class="row align-items-center pb-5">
        <div class="col-sm-6">
          <em
            >&copy; 2020 <span class="mini_bullet">•</span> Avada Consultant
            <span class="mini_bullet">•</span> Powered by WordPress</em
          >
        </div>
        <div class="col-sm-3">
          <em>Call Us (555) 802-1234</em>
        </div>
        <div class="col-sm-3 text-end">
          <em>info@yourcompany.com</em>
        </div>
      </div>
      <VueBotUI
        :messages="data"
        :options="botOptions"
        @init="botStart"
        @msg-send="msgSend"
      />
    </div>
  </div>
</template>

<script>
import { VueBotUI } from "vue-bot-ui";

export default {
  name: "FooterBottom",
  components: {
    VueBotUI,
  },
  data() {
    return {
      data: [],
      botOptions: {
        botTitle: "Avada Kedavra Bot",
        colorScheme: "#f76210",
        msgBubbleBgBot: "#424242",
        msgBubbleColorBot: "#fff",
        msgBubbleBgUser: "#f76210",
        msgBubbleColorUser: "#fff",
      },
    };
  },
  methods: {
    botStart() {
      this.botTyping = true;
      setTimeout(() => {
        this.botTyping = false;
        this.data.push({
          agent: "bot",
          type: "text",
          text: "Hello. How can I help you?",
        });
      }, 1000);
    },
    msgSend(value) {
      this.data.push({
        agent: "user",
        type: "text",
        text: value.text,
      });
      this.getResponse();
    },
    getResponse() {
      this.botTyping = true;
      setTimeout(() => {
        this.botTyping = false;
        this.data.push({
          agent: "bot",
          type: "text",
          text: "Chat is temporarily unavailable. Try again later, or ask Ciro Cusati",
        });
      }, 1000);
    },
  },
};
</script>

<style lang="scss" scoped>
em {
  font-size: 14px;

  .mini_bullet {
    font-size: 20px;
  }
}
</style>