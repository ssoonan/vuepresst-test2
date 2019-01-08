<template>
  <v-app light>
    <v-content>
      <v-container>
        <v-layout row wrap align-center>
          <header>
            {{#if readingTime}}
            Reading Time {{readingTime}} min | {{/if}}

            published on the {{date postDate}}

            {{#if lastUpdated}}
            and last updated {{date lastUpdated}}
            {{/if}}
          </header>
          <article>
            <Content :custome="false" />
          </article>
        </v-layout>
      </v-container>
    </v-content>
  </v-app>
</template>
