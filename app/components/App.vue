<template>
    <Page>
        <!-- <ActionBar title="Welcome to NativeScript-Vue!" android:flat="true"/> -->
        <TabView android:tabBackgroundColor="#53ba82"
                 android:tabTextColor="#c4ffdf"
                 android:selectedTabTextColor="#ffffff"
                 androidSelectedTabHighlightColor="#ffffff" >

            <TabViewItem title="Tab 1">
                <GridLayout columns="*,*,*" rows="*,*,*,*,*,*,*,*">
                    <Label class="h1" text="Where To?" col="1" row="0"/>
                    <TextField class="m-x-auto" :text="textFieldValue" hint="Current Location" col="1" row="1" />
                    <TextField class="m-x-auto" :text="textFieldValue" hint="Destination" col="1" row="2" />
                </GridLayout>
                
                <!-- <FlexboxLayout flexDirection="column" 
                                alignItems="center"
                                justifyConten="space-between" >
                                
                    <Label class="h1 m-y-15" text="Where To?" col="1" row="0"/>
                    <Label class="h2 p-l-20 m-b-30 " alignSelf="flex-start" text="Current Location" col="1" row="0"/>
                    <TextField class="p-y-5 p-x-15 myInput" :text="textFieldValue" hint="Current Location" col="1" row="1" />
                    <TextField class="p-y-5 p-x-15 myInput" :text="textFieldValue" hint="Destination" col="1" row="2" />

                </FlexboxLayout> -->
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
    .myInput {
        margin: 0 auto;
        border: solid 2px #2e3140;
    }
</style>
