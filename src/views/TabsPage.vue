<template>
    <ion-page>
        <ion-tabs>
            <ion-router-outlet></ion-router-outlet>
            <ion-tab-bar slot="bottom">
                <ion-tab-button tab="discovery-of-the-day" href="/tabs/discovery-of-the-day">
                    <ion-icon :icon="calendar" />
                </ion-tab-button>

                <ion-tab-button tab="artworks-list" href="/tabs/artworks-list">
                    <ion-icon :icon="list" />
                </ion-tab-button>

                <ion-tab-button tab="map" href="/tabs/map">
                    <ion-icon :icon="map" />
                </ion-tab-button>

                <ion-tab-button tab="collection" href="/tabs/collection">
                    <ion-icon :icon="book" />
                </ion-tab-button>

                <ion-tab-button tab="more" href="/tabs/more">
                    <ion-icon :icon="ellipsisHorizontalCircle" />
                </ion-tab-button>
            </ion-tab-bar>
        </ion-tabs>
    </ion-page>
</template>

<script setup lang="ts">
/* Importing the toolbar's CSS here so it's done once and for all */
import { IonTabBar, IonTabButton, IonTabs, IonIcon, IonPage, IonRouterOutlet } from '@ionic/vue';
import { list, map, book, ellipsisHorizontalCircle, calendar } from 'ionicons/icons';
</script>

<style>
@import url("@/theme/TopToolbar.css");

ion-tab-bar {
    height: 10%;
    border: 0;
    --background: var(--toolbar-purple);
}

ion-icon {
    font-size: 27px;
}
</style>
