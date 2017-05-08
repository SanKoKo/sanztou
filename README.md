# sanztou
zawgyi to uni or uni to zawgyi

ကၽြန္ေတာ္ကိုယ္တိုင္သံုးဖို႔ ဒီ sanztou library ေလးကိုေရးလိုက္တာပါ။ ဒါေပမဲ့ ကၽြန္ေတာ့ညီငယ္ Oscar Myo Min ရဲ႕ တိုက္တြန္းမႈ႕ေၾကာင့္ Public ေပးသံုးလိုက္တာပါ။ ဒါေၾကာင့္ ဒီ lib က အရမ္းအဆင္ေျပလွတယ္မဟုတ္ေပမဲ့ အထုိက္အေလ်ာက္ေတာ့ ေဇာ္ဂ်ီကေန ယူနီ၊ ယူနီကေန ေဇာ္ဂ်ီကို ေျပာင္းႏုိင္ေအာင္ အေထာက္အထူျပဳႏိုင္ပါတယ္။ ဒီ lib ကို အခမဲ့ အသံုးျပဳႏိုင္ပါတယ္။ ဒါေပမဲ့ အသံုးျပဳတဲ့အခါမွာေတာ့ credit ေပးေစလိုပါတယ္။ lib အသံုးျပဳပံုကိုေအာက္မွာေဖာ္ျပေပးထားပါတယ္။

Zawgyi နဲ႔ေရးထားတာကို Unicode ေျပာင္းျပခ်င္တယ္ဆိုရင္ ပံုမွန္ေရးေနၾကပံုစံအတိုင္းနဲ႔ေရးမယ္ဆိုရင္ ေအာက္အတိုင္းေရးရံုပါပဲ။ “mm3.ttf” ဆိုတာကေတာ့ unicode font ျဖစ္ပါတယ္။ အဲ့ဒီေဖာင့္ကို assest folder ထဲ ထည့္ေပးထားရပါမယ္။ “mm3.ttf” ေဖာင့္ေနရာမွာ သင့္ Unicode font ကို အစားထိုးအသံုးျပဳႏိုင္ပါတယ္။

SanZtoU sanZtoU = new SanZtoU(this);
String mystring = (String) sanZtoU.ZawGyiToUni("ေဖာ္ဂ်ီျဖင့္ေရးထားပါတယ္",true);


Typeface font = Typeface.createFromAsset(getAssets(),"mm3.ttf");
TextView tv = (TextView) findViewById(R.id.tv);
tv.setText(mystring);
tv.setTypeface(font);

Unicode နဲ႔ေရးထားတာကို Zawgyi ေျပာင္းျပခ်င္တယ္ဆိုရင္ ပံုမွန္ေရးေနၾကပံုစံအတိုင္းနဲ႔ေရးမယ္ဆိုရင္ ေအာက္အတိုင္းေရးရံုပါပဲ။ “zg.TTF” ဆိုတာကေတာ့ unicode font ျဖစ္ပါတယ္။ အဲ့ဒီေဖာင့္ကို assest folder ထဲ ထည့္ေပးထားရပါမယ္။ “zg.TTF” ေဖာင့္ေနရာမွာ သင့္ Zawgyi font ကို အစားထိုးအသံုးျပဳႏိုင္ပါတယ္။ false value ကိုအသံုးျပဳရတာ သတိထားမိရင္ ရပါၿပီ။ က်န္တာ အေပၚကအတိုင္းပါပဲ။

SanZtoU sanZtoU = new SanZtoU(this);
String mystring = (String) sanZtoU.ZawGyiToUni("ယူနီျဖင့္ေရးထားပါတယ္",false);


Typeface font = Typeface.createFromAsset(getAssets(),"zg.TTF");
TextView tv = (TextView) findViewById(R.id.tv);
tv.setText(mystring);
tv.setTypeface(font);

အထက္ကျပထားတဲ့အတိုင္း တစ္ခုခ်င္းစီအတြက္အသံုးျပဳႏိုင္တဲ့အျပင္ Activity တစ္ခုလံုးအတြက္ Coding တစ္ေၾကာင္းတည္းနဲ႔ zawgyi to uni, uni to zawgyi အသံုးျပဳႏိုင္ပါတယ္။ Oncreate() ကြင္းေနာက္ဆံုးမွာ ထည့္သံုးပါ။ Typeface သံုးရန္မလိုပါ။ အသံုးျပဳပံုကိုေအာက္မွာေဖာ္ျပထားပါတယ္။

zawgyi နဲ႔ေရးထားတာကို unicode ျပခ်င္တယ္ဆိုရင္ ေအာက္ပါအတိုင္းေရးပါ။ “mm3.ttf” ဆိုကေတာ့ သင့္ assest folder ထဲမွာရွိတဲ့ font နာမည္ပါ။ true ဆိုတာကေတာ့ zawgyi ကေန uni ေျပာင္းမယ္ဆိုတဲ့အဓိပၸာယ္ပါ။ 

new SanZtoU(this).ForceToUni("mm3.ttf", true);

တကယ္လို႔ uni နဲ႔ေရးထားတာကို uni ပဲ Force ျပခ်င္တယ္ဆိုရင္ေတာ့ ေအာက္ပါအတုိင္းေရးပါ။

new SanZtoU(this).ForceToUni("mm3.ttf", null);


unicode နဲ႔ေရးထားတာကို zawgyi ျပခ်င္တယ္ဆိုရင္ ေအာက္ပါအတိုင္းေရးပါ။ “zg.TTF” ဆိုကေတာ့ သင့္ assest folder ထဲမွာရွိတဲ့ font နာမည္ပါ။ false ဆိုတာကေတာ့ uni ကေန uni မဟုတ္တဲ့ zawgyi ေျပာင္းမယ္ဆိုတဲ့အဓိပၸာယ္ပါ။ 
new SanZtoU(this). ForceToZawGyi("zg.TTF", false);

အကယ္၍ zawgyi နဲ႔ေရးထားတာကို zawgyi ပဲ Force ခ်င္တယ္ဆိုရင္ေတာ့ ေအာက္ပါအတုိင္းေရးပါ။
new SanZtoU(this). ForceToZawGyi("zg.TTF", null);

Xtreme mode
Xtreme mode ကို update ျပဳလုပ္ေပးထားပါတယ္။ Xtreme mode ဆိုတာကေတာ့ Zawgyi or Uni ေတြကို အတင္းအၾကပ္ Force လုပ္ၿပီး ျပေစျခင္းျဖစ္ပါတယ္။ အမ်ဳိးမ်ဳိးေသာ ဖုန္းမ်ားအတြက္ စာဖတ္လို႔ ရဖို႔ကို အဓိက ရည္ရြယ္ပါတယ္။ Xtreme mode ကိုသံုးရန္အတြက္ “san.ttf” font ကို assest folder ထဲမွာ ထည့္ထားဖို႔လိုအပ္ပါတယ္။ Font ဆရာႀကီးေတြ အတြက္မရည္ရြယ္ပါဘူး။ 
Zawgyi ေဖာင့္နဲ႔ ေရးထားတဲ့ စာကို Zawgyi ပဲ Override ျပခ်င္တယ္ဆိုရင္။ true ဆိုတာကေတာ့ Zawgyi font နဲ႔ေရးထားတာလို႔ ဆိုလိုပါတယ္။
SanZtoU sanZtoU = new SanZtoU(this);
String mystring = (String) sanZtoU.XtremeZawGyi("ေဇာ္ဂ်ီျဖင့္ေရးထားသည္။",true);


Typeface font = Typeface.createFromAsset(getAssets(),"san.ttf");
TextView tv = (TextView) findViewById(R.id.tv);
tv.setText(mystring);
tv.setTypeface(font);

Uni နဲ႔ ေရးထားတဲ့ စာကို Zawgyi ပဲ Override ျပခ်င္တယ္ဆိုရင္။ false ဆိုတာကေတာ့ Uni နဲ႔ေရးထားတာလို႔ ဆိုလိုပါတယ္။
SanZtoU sanZtoU = new SanZtoU(this);
String mystring = (String) sanZtoU.XtremeZawGyi("ယူနီျဖင့္ေရးထားသည္",false);


Typeface font = Typeface.createFromAsset(getAssets(),"san.ttf");
TextView tv = (TextView) findViewById(R.id.tv);
tv.setText(mystring);
tv.setTypeface(font);


Activity တစ္ခုလံုးကို Xtreme လုပ္ခ်င္တယ္ဆိုရင္ေတာ့ ေအာက္ပါအတုိင္း ေရးႏိုင္ပါတယ္။

Zawgyi
Zawgyi Font နဲ႔ေရးထားတာကို Zawgyi ပဲ Xtreme လုပ္ခ်င္တယ္ဆိုရင္ ….
new SanZtoU(this).XtremlyForceToZawgyi(true);

Uni  နဲ႔ေရးထားတာကို Zawgyi  Xtreme လုပ္ခ်င္တယ္ဆိုရင္ ….
new SanZtoU(this).XtremlyForceToZawgyi(false);

Uni
Uni  နဲ႔ေရးထားတာကို Uni ပဲ Xtreme လုပ္ခ်င္တယ္ဆိုရင္ ….
new SanZtoU(this).XtremlyForceToUni(true);

Zawgyi  နဲ႔ေရးထားတာကို Uni  Xtreme လုပ္ခ်င္တယ္ဆိုရင္ ….
new SanZtoU(this).XtremlyForceToUni(false);


## new updated
ကၽြန္ေတာ့ library မွာ ေနာက္ထပ္ Feature တစ္ခု ထပ္ထည့္ေပးထားပါတယ္။ အဲ့ဒါကေတာ့ Font Chooser ပါ။ User ကို ေဖာင့္ ေရြးခ်ယ္ေစဖို႔နဲ႔ သူေရြးခ်ယ္ထားတာကို ျပဖို႔ ပံုမွန္အားျဖင့္ ကၽြန္ေတာ္တို႔ေတြ  သူေရြးထားတာကို သိမ္းထားဖို႔ လုိပါတယ္။ 

အခုအသစ္ထပ္ထဲ့လိုက္တဲ့ feature က အဲ့ဒီ ဒုကၡေတြကို ကင္းေစမွာပါ။ အရမ္းလြယ္ပါတယ္။


## update feature ကိုသံုးမယ္ဆိုရင္ေတာ့ အရင္ဦးဆံုး ကိုယ့္ project ထဲက စာေတြကို ဘာ Font နဲ႔ေရးထားတယ္ဆိုတာ အရင္ ေအာက္ပါအတုိင္း သတ္မွတ္ေပးရပါမယ္။
BuildDefaultFont.setProjectDefaultFont(DefaultFont.UNICODE); // uni ဆို uni၊ zawgyiဆို zawgyi သတ္မွတ္ရပါမယ္။
ၿပီးရင္ေတာ့ ေအာက္ပါအတုိင္း ေဖာ္ျပည့္ data ရယ္ view ရယ္ကို ထည့္လိုက္ယံုပါပဲ။

new SanZtoU(this).autoTextFace(data,tv);

Font chooser ရဲ႕ button ႏွိပ္လိုက္တာသိခ်င္ရင္ 
startActivityForResult(intent,requestcode); နဲ႔ စစ္ေဆးႏိုင္ပါတယ္။

ေနာက္ဆံုးအေနနဲ႔ 
Manifest ထဲမွာ ေအာက္ပါအတုိင္း ေၾကျငာဖို႔လိုပါတယ္။ <activity android:name="san.zgyi.uni.MessageView"/>

video tutorial ကို ကၽြန္ေတာ့ရဲ႕ facebook sandevelopment page ထဲမွာ တင္ေပးထားပါတယ္။

library အသံုးျပဳရအဆင္မေျပတာရွိရင္ေသာ္လည္းေကာင္း၊ အၾကံအဥာဏ္ေပးလိုလွ်င္ေသာ္လည္းေကာင္း ကၽြန္ေတာ့္ကိုဆက္သြယ္ႏိုင္ပါတယ္။
San Software Development Training
အမွတ္ - ၂၃(စီ) ၊ ပထမထပ္၊ သံလမ္း၊ လိႈင္ၿမိဳ႕နယ္။ ရန္ကုန္။
ဖုန္း - ၀၉ ၂၅၀၀ ၅၂၃၀၁
လစဥ္ သင္တန္း တန္းခဲြရွိပါသည္။ 	
သင္ၾကားေပးေသာဘာသာရပ္မ်ား -
Android Basic
Android Advance
Ios developing
C#.Net
ေက်းဇူးတင္ပါသည္။
