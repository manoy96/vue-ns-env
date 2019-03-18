<template>
  <Page>
    <!-- <ActionBar title="Welcome to NativeScript-Vue!" android:flat="true"/> -->
    <TabView
      android:tabBackgroundColor="#53ba82"
      android:tabTextColor="#c4ffdf"
      android:selectedTabTextColor="#ffffff"
      androidSelectedTabHighlightColor="#ffffff"
      tabTextFontSize="18"
      selectedTabTextColor="#ffffff"
      tabTextColor="#2e3140"
    >
      <TabViewItem title="Plan" >
        <GridLayout columns="*" rows="*,*,*,*,*,*,*,*,*,*,*">
          <Label class="h1 m-x-auto" text="Where To?" col="0" row="0"/>
          <Label class="h2 m-l-30" text="Starting Point" col="0" row="1"/>
          <TextField
            class="m-x-auto p-l-15 myInput"
            :text="textFieldValue"
            hint="Current Location"
            col="0"
            row="2"
          />
          <Label class="h2 m-l-30" text="Destination" col="0" row="3"/>
          <TextField
            class="m-x-auto p-l-15 myInput"
            :text="textFieldValue"
            hint="Destination"
            col="0"
            row="4"
          />

          <StackLayout class="hr-light m-20" col="0" row="5"></StackLayout>

          <Label class="h2 m-l-30" text="Recent Trips" col="0" row="6"/>
          <Label class="h2 m-x-auto myRecent" text="Utah Valley University" col="0" row="7" />
          <Label class="h2 m-x-auto myRecent" text="Walmart" col="0" row="8" />
          <Button class="h2 myButton" text="GO" @tap="onButtonTap" col="0" row="9" />
        </GridLayout>

        <!-- <FlexboxLayout flexDirection="column" 
                                alignItems="center"
                                justifyConten="space-between" >
                                
                    <Label class="h1 m-y-15" text="Where To?" col="1" row="0"/>
                    <Label class="h2 p-l-20 m-b-30 " alignSelf="flex-start" text="Current Location" col="1" row="0"/>
                    <TextField class="p-y-5 p-x-15 myInput" :text="textFieldValue" hint="Current Location" col="1" row="1" />
                    <TextField class="p-y-5 p-x-15 myInput" :text="textFieldValue" hint="Destination" col="1" row="2" />

        </FlexboxLayout>-->
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
      msg: "Where To?"
    };
  }
};
</script>

<style scoped>
ActionBar {
  background-color: #c11327;
  color: #ffffff;
}
tabView {
   tab-background-color: #c11327;
}

.message {
  vertical-align: center;
  text-align: center;
  font-size: 20;
  color: #333333;
}
.myInput {
  border-width: 2;
  border-color: #86858c;
  border-radius: 30;
}
.myRecent {
   border-width: 2;
   border-top-color: #c9c9c9;
   width: 90%;
   text-align: center;
}
.myButton {
   width: 90%;
   background-color: #86858c;
   color: #ffffff;
   border-radius: 15;
}
</style>
