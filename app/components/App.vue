<template>
    <Page>
        <ActionBar title="Welcome to NativeScript-Vue!" android:flat="true"/>
        <TabView android:tabBackgroundColor="#53ba82"
                 android:tabTextColor="#c4ffdf"
                 android:selectedTabTextColor="#ffffff"
                 androidSelectedTabHighlightColor="#ffffff" >

            <TabViewItem title="Tab 1">
                <GridLayout columns="*,*,*" rows="*,*,*,*,*,*,*,*">
                    <!-- <Label class="message" :text="msg" col="1" row="0"/> -->
                    <Label text="Where To?" class="message" col="1" row="0"/>
                    <TextField class="myInput" :text="textFieldValue" hint="Current Location" col="1" row="1" />
                    <TextField :text="textFieldValue" hint="Destination" col="1" row="2" />
                </GridLayout>
            </TabViewItem>

            <TabViewItem title="Tab 2">
                <GridLayout columns="*" rows="*">
                    <Label class="message" text="Tab 2 Content" col="0" row="0"/>
                </GridLayout>
            </TabViewItem>

            <TabViewItem title="Tab 3">
                <GridLayout columns="*" rows="*">
                    <Label class="message" text="Tab 3 Content" col="0" row="0"/>
                </GridLayout>
            </TabViewItem>
        </TabView>
    </Page>
</template>

<script >
  export default {
    data() {
      return {
        msg: 'Where To?'
      }
    }
  }
</script>

<style scoped>
    ActionBar {
        background-color: #c11327;
        color: #ffffff;
    }

    .message {
        vertical-align: center;
        text-align: center;
        font-size: 20;
        color: #333333;
    }
    .myinput {
        margin: 0 auto;
        border-bottom: solid 2px #2e3140;
    }
</style>
