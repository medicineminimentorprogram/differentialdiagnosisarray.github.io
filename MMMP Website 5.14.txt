<template>
  <div>
    <button @click="toggleLists" :class="{ large: large }">Toggle lists</button>
        <!-- Image 1 is also known as "Cardiovascular Fundamentals" -->
    <img v-if="showimage1" src="https://i.imgur.com/bQeL6jM.png" alt="Image 1" height="800" width= "625" class="image1" />
        <!-- Image 2 is also known as "Heart Icon" -->
    <img v-if="showimage2" src="https://i.imgur.com/t1mMMUg.png" alt="Image 2" height="150" width= "150" class="image2" />
    <button @click="toggleImages3" class="second-button">Toggle Image 3</button>
        <!-- Image 3 is also known as "Palpitation Phrase" -->    
    <img v-if="showimage3" src="https://i.imgur.com/WY4uKAt.png" alt="Image 3" height="75" width= "300" class="image3" />
        <!-- Image 4 is also known as "Palpitation  Button" -->
    <img v-if="showimage4" src="https://i.imgur.com/v0EwMuF.png" alt="Image 4" height="150" width= "150" class="image4" />
    <!-- Heart - Palpitation -->
    <img v-if="showimage5" src="https://i.imgur.com/QWkQZNJ.png" alt="Image 5" height="275" width= "250" class="image5" />
    <button @click="toggleImages4" class="third-button">Toggle Image 6</button> 
        <!-- Image 6 is also known as "Chest Pain Phrase" -->    
    <img v-if="showimage6" src="https://i.imgur.com/xeiJB7j.png" alt="Image 6" height="50" width= "225" class="image6" />
        <!-- Image 7 is also known as "Chest Pain Button" -->
    <img v-if="showimage7" src="https://i.imgur.com/QeEwk2T.png" alt="Image 7" height="150" width= "150" class="image7" />
    <!-- Heart - Chest Pain -->
    <img v-if="showimage8" src="https://i.imgur.com/1wdcIsR.png" alt="Image 8" height="400" width= "20" class="image8" />
    <button @click="toggleImages5" class="fourth-button">Toggle Image 9</button>
        <!-- Image 9 is also known as "Congenital Phrase" -->    
    <img v-if="showimage9" src="https://i.imgur.com/TiRrdiq.png" alt="Image 9" height="80" width= "350" class="image9" />
        <!-- Image 10 is also known as "Congenital  Button" -->
    <img v-if="showimage10" src="https://i.imgur.com/y89hUep.png" alt="Image 10" height="150" width= "150" class="image10" />
    <!-- Heart - Congenital -->
    <img v-if="showimage11" src="https://i.imgur.com/betxp92.png" alt="Image 11" height="20" width= "500" class="image11" />
    <button @click="toggleImages6" class="fifth-button">Toggle Image 12</button>
        <!-- Image 12 is also known as "Fever Phrase" -->    
    <img v-if="showimage12" src="https://i.imgur.com/kre3Dpw.png" alt="Image 12" height="50" width= "150" class="image12" />
        <!-- Image 13 is also known as "Fever  Button" -->
    <img v-if="showimage13" src="https://i.imgur.com/z5BLgyB.png" alt="Image 13" height="150" width= "150" class="image13" />
    <!-- Heart - Fever -->
    <img v-if="showimage14" src="https://i.imgur.com/qfWwWOv.png" alt="Image 14" height="275" width= "375" class="image14" />
    <button @click="toggleImages7" class="sixth-button">Toggle Image 15</button>
        <!-- Image 15 is also known as "Jugular Venous Distention Phrase" -->    
    <img v-if="showimage15" src="https://i.imgur.com/S9ziwYq.png" alt="Image 15" height="125" width= "325" class="image15" />
        <!-- Image 16 is also known as "Jugular Venous Distention  Button" -->
    <img v-if="showimage16" src="https://i.imgur.com/IDO7ghQ.png" alt="Image 16" height="150" width= "150" class="image16" />
    <!-- Heart - Jugular Venous Distention -->
    <img v-if="showimage17" src="https://i.imgur.com/b9qHXXT.png" alt="Image 17" height="250" width= "200" class="image17" />
    <button @click="toggleImages8" class="seventh-button">Toggle Image 18</button>
        <!-- Image 18 is also known as "Lower Limb Low Blood Pressure Phrase" -->    
    <img v-if="showimage18" src="https://i.imgur.com/H00Snyg.png" alt="Image 18" height="100" width= "225" class="image18" />
        <!-- Image 19 is also known as "Lower Limb Low Blood Pressure  Button" -->
    <img v-if="showimage19" src="https://i.imgur.com/6aFdT6a.png" alt="Image 19" height="150" width= "150" class="image19" />
    <!-- Heart - Lower Limb Low Blood Pressure -->
    <img v-if="showimage20" src="https://i.imgur.com/PCT2flJ.png" alt="Image 20" height="250" width= "300" class="image20" />
    <button @click="toggleImages9" class="eighth-button">Toggle Image 21</button>
        <!-- Image 21 is also known as "Murmur Phrase" -->    
    <img v-if="showimage21" src="https://i.imgur.com/hJ4Bc3y.png" alt="Image 21" height="75" width= "275" class="image21" />
        <!-- Image 22 is also known as "Murmur Button" -->
    <img v-if="showimage22" src="https://i.imgur.com/nFNytml.png" alt="Image 22" height="150" width= "150" class="image22" />
    <!-- Heart - Murmur -->
    <img v-if="showimage23" src="https://i.imgur.com/B7f0tJD.png" alt="Image 23" height="400" width= "20" class="image23" />
    <button @click="toggleImages10" class="ninth-button">Toggle Image 24</button>
        <!-- Image 24 is also known as "Peripheral Edema Phrase" -->    
    <img v-if="showimage24" src="https://i.imgur.com/whQcyva.png" alt="Image 24" height="100" width= "225" class="image24" />
        <!-- Image 25 is also known as "Peripheral Edema  Button" -->
    <img v-if="showimage25" src="https://i.imgur.com/K8p6IrL.png" alt="Image 25" height="150" width= "150" class="image25" />
    <!-- Heart - Peripheral Edema -->
    <img v-if="showimage26" src="https://i.imgur.com/1E9BIL3.png" alt="Image 17" height="225" width= "350" class="image26" />
    <button @click="toggleImages11" class="tenth-button">Toggle Image 27</button>
        <!-- Image 27 is also known as "Syncope Phrase" -->    
    <img v-if="showimage27" src="https://i.imgur.com/OXq5Yk4.png" alt="Image 27" height="75" width= "250" class="image27" />
        <!-- Image 28 is also known as "Syncope  Button" -->
    <img v-if="showimage28" src="https://i.imgur.com/lDoAYQI.png" alt="Image 28" height="150" width= "150" class="image28" />
    <!-- Heart - Syncope -->
    <img v-if="showimage29" src="https://i.imgur.com/Bh80jp0.png" alt="Image 29" height="200" width= "350" class="image29" />
    <button @click="toggleImages12" class="eleventh-button">Toggle Image 30</button>
        <!-- Image 30 is also known as "Weight Loss Phrase" -->    
    <img v-if="showimage30" src="https://i.imgur.com/lT0JvP1.png" alt="Image 30" height="50" width= "250" class="image30" />
        <!-- Image 31 is also known as "Weight Loss  Button" -->
    <img v-if="showimage31" src="https://i.imgur.com/M1x4dOX.png" alt="Image 31" height="150" width= "150" class="image31" />
    <!-- Heart - Weight Loss -->
    <img v-if="showimage32" src="https://i.imgur.com/betxp92.png" alt="Image 32" height="20" width= "500" class="image32" />
    <button @click="toggleImages13" class="twelfth-button">Toggle Image 33</button>
    <!-- Substernal Chest Pain Phrase -->
    <img v-if="showimage33" src="https://i.imgur.com/f82qlSo.png" alt="Image 33" height="125" width= "275" class="image33" />    
    <!-- Substernal Chest Pain Button-->
    <img v-if="showimage34" src="https://i.imgur.com/vHhZGUy.png" alt="Image 34" height="150" width= "150" class="image34" />      
    <button @click="toggleImages15" class="fourteenth-button">Toggle Image 39</button>     
    <!-- Cyanosis Phrase -->
    <img v-if="showimage39" src="https://i.imgur.com/aIaWpVG.png" alt="Image 39" height="125" width= "250" class="image39" />    
    <!-- Cyanosis Button-->
    <img v-if="showimage40" src="https://i.imgur.com/5gAbaYX.png" alt="Image 40" height="150" width= "150" class="image40" /> 
    <button @click="toggleImages16" class="fifteenth-button">Toggle Image 42</button>       
    <!-- Tearing Pain Phrase -->
    <img v-if="showimage42" src="https://i.imgur.com/Ao0kKqD.png" alt="Image 42" height="125" width= "250" class="image42" />    
    <!-- Tearing Pain Button-->
    <img v-if="showimage43" src="https://i.imgur.com/8aewSf9.png" alt="Image 43" height="150" width= "150" class="image43" />  
    <button @click="toggleImages17" class="sixteenth-button">Toggle Image 45</button>       
    <!-- Sharp Chest Pain Phrase -->
    <img v-if="showimage45" src="https://i.imgur.com/QOqwKjM.png" alt="Image 45" height="125" width= "250" class="image45" />    
    <!-- Sharp Chest Pain Button-->
    <img v-if="showimage46" src="https://i.imgur.com/ycIX2cw.png" alt="Image 46" height="150" width= "150" class="image46" />      
    <button @click="toggleImages18" class="seventeenth-button">Toggle Image 48</button>         
    <!-- Low Pitch Holosystolic Phrase -->
    <img v-if="showimage48" src="https://i.imgur.com/gLM8kVA.png" alt="Image 48" height="150" width= "350" class="image48" />    
    <!-- Low Pitch Holosystolic Button-->
    <img v-if="showimage49" src="https://i.imgur.com/hWhLr83.png" alt="Image 49" height="150" width= "150" class="image49" />    
    <button @click="toggleImages19" class="eightteenth-button">Toggle Image 51</button>           
    <!-- CREAM Phrase -->
    <img v-if="showimage51" src="https://i.imgur.com/oGCyfh4.png" alt="Image 51" height="75" width= "250" class="image51" />    
    <!-- CREAM Button-->
    <img v-if="showimage52" src="https://i.imgur.com/Pb7YPq5.png" alt="Image 52" height="150" width= "150" class="image52" />  
    <button @click="toggleImages20" class="nineteenth-button">Toggle Image 54</button>       
    <!-- Red LL Phrase -->
    <img v-if="showimage54" src="https://i.imgur.com/HHn53eG.png" alt="Image 54" height="100" width= "250" class="image54" />    
    <!-- Red LL Button-->
    <img v-if="showimage55" src="https://i.imgur.com/I1XGEUn.png" alt="Image 55" height="150" width= "150" class="image55" /> 
    <button @click="toggleImages21" class="twentieth-button">Toggle Image 57</button>               
    <!-- Decreased Heart Sound Phrase -->
    <img v-if="showimage57" src="https://i.imgur.com/a9Fnuf2.png" alt="Image 57" height="125" width= "325" class="image57" />    
    <!-- Decreased Heart Sound Button-->
    <img v-if="showimage58" src="https://i.imgur.com/YTOGHoc.png" alt="Image 58" height="150" width= "150" class="image58" /> 
    <button @click="toggleImages22" class="twenty-first-button">Toggle Image 60</button>       
    <!-- Tachycardia Phrase -->
    <img v-if="showimage60" src="https://i.imgur.com/VVi2Cx0.png" alt="Image 60" height="50" width= "250" class="image60" />    
    <!-- Tachycardia Button-->
    <img v-if="showimage61" src="https://i.imgur.com/z7YohnV.png" alt="Image 61" height="150" width= "150" class="image61" /> 
    <button @click="toggleImages23" class="twenty-second-button">Toggle Image 63</button>     
    <!-- Bradycardia Phrase -->
    <img v-if="showimage63" src="https://i.imgur.com/XOPXS4q.png" alt="Image 63" height="50" width= "250" class="image63" />    
    <!-- Bradycardia Button-->
    <img v-if="showimage64" src="https://i.imgur.com/xhjQgP7.png" alt="Image 64" height="150" width= "150" class="image64" />    
    <button @click="toggleImages24" class="twenty-third-button">Toggle Image 66</button>          
    <!-- Back Pain Phrase -->
    <img v-if="showimage66" src="https://i.imgur.com/woAfPoL.png" alt="Image 66" height="50" width= "200" class="image66" />    
    <!-- Back Pain Button-->
    <img v-if="showimage67" src="https://i.imgur.com/1k04VEH.png" alt="Image 67" height="150" width= "150" class="image67" /> 
    <button @click="toggleImages25" class="twenty-fourth-button">Toggle Image 69</button>                     
    <!-- Baseline Asymptomatic Phrase -->
    <img v-if="showimage69" src="https://i.imgur.com/d2NlzY5.png" alt="Image 69" height="100" width= "325" class="image69" />    
    <!-- Baseline Asymptomatic Button-->
    <img v-if="showimage70" src="https://i.imgur.com/sjiuBEm.png" alt="Image 70" height="150" width= "150" class="image70" />   
    <button @click="toggleImages26" class="twenty-fifth-button">Toggle Image 72</button>                     
    <!-- Hypotension Phrase -->
    <img v-if="showimage72" src="https://i.imgur.com/UoOosqD.png" alt="Image 72" height="75" width= "375" class="image72" />    
    <!-- Hypotension Button-->
    <img v-if="showimage73" src="https://i.imgur.com/cD66Cgs.png" alt="Image 73" height="150" width= "150" class="image73" /> 
    <button @click="toggleImages27" :class="{ large2: large2 }" class="twenty-sixth-button">Toggle Image 75</button>    
    <!-- Uremic Pericarditis Card -->
    <img v-if="showimage75" src="https://i.imgur.com/dT44UZu.png" alt="Image 75" height="400" width= "650" class="image75" />
    <!-- Uremic Pericarditis Button -->
    <img v-if="showimage76" src="https://i.imgur.com/SwDF3yG.png" alt="Image 76" height="150" width= "325" class="image76" />            
    <button @click="toggleImages28" :class="{ large3: large3 }" class="twenty-seventh-button">Toggle Image 77</button>    
    <!-- Chagas Disease Card -->
    <img v-if="showimage77" src="https://i.imgur.com/deZkfQh.png" alt="Image 77" height="400" width= "700" class="image77" />
    <!-- Chagas Disease Button -->
    <img v-if="showimage78" src="https://i.imgur.com/p8tmJcC.png" alt="Image 78" height="150" width= "275" class="image78" />     
    <button @click="toggleImages29" :class="{ large4: large4 }" class="twenty-eighth-button">Toggle Image 79</button>    
    <!-- Infective Endocarditis Card -->
    <img v-if="showimage79" src="https://i.imgur.com/CSlr7GE.png" alt="Image 79" height="400" width= "6500" class="image79" />
    <!-- Infective Endocarditis Button -->
    <img v-if="showimage80" src="https://i.imgur.com/8nxKxyV.png" alt="Image 80" height="150" width= "350" class="image80" />          
    <button @click="toggleImages30" :class="{ large5: large5 }" class="twenty-ninenth-button">Toggle Image 81</button>    
    <!-- Atrial Myxoma Card -->
    <img v-if="showimage81" src="https://i.imgur.com/MCpmHjE.png" alt="Image 81" height="400" width= "850" class="image81" />
    <!-- Atrial Myxoma Button -->
    <img v-if="showimage82" src="https://i.imgur.com/sO2rCOF.png" alt="Image 82" height="150" width= "250" class="image82" />      
    <button @click="toggleImages31" :class="{ large6: large6 }" class="thirtieth-button">Toggle Image 83</button>   
    <!-- Deep Venous Thrombosis Card -->
    <img v-if="showimage83" src="https://i.imgur.com/CusPxx7.png" alt="Image 83" height="600" width= "500" class="image83" />      
    <!-- Deep Venous Thrombosis Button -->
    <img v-if="showimage84" src="https://i.imgur.com/FZTxxpR.png" alt="Image 84" height="150" width= "375" class="image84" />   
    <button @click="toggleImages32" :class="{ large7: large7 }" class="thirty-first-button">Toggle Image 85</button>    
    <!-- Kawasakis Disease Card -->
    <img v-if="showimage85" src="https://i.imgur.com/9ELnUVl.png" alt="Image 85" height="400" width= "650" class="image85" />
    <!-- Kawasakis Disease Button -->
    <img v-if="showimage86" src="https://i.imgur.com/LvU9pDg.png" alt="Image 86" height="150" width= "300" class="image86" />      
    <button @click="toggleImages33" :class="{ large8: large8 }" class="thirty-second-button">Toggle Image 87</button>    
    <!-- Cardiac Tamponade Card -->
    <img v-if="showimage87" src="https://i.imgur.com/DfMwQS4.png" alt="Image 87" height="400" width= "625" class="image87" />
    <!-- Cardiac Tamponade Button -->
    <img v-if="showimage88" src="https://i.imgur.com/MW80DXn.png" alt="Image 88" height="150" width= "350" class="image88" />     
    <button @click="toggleImages34" :class="{ large9: large9 }" class="thirty-third-button">Toggle Image 89</button> 
    <!-- Pericardial Effusion Card -->
    <img v-if="showimage89" src="https://i.imgur.com/WnuBp38.png" alt="Image 89" height="400" width= "550" class="image89" />         
    <!-- Pericardial Effusion Button -->
    <img v-if="showimage90" src="https://i.imgur.com/cVxP5rz.png" alt="Image 90" height="150" width= "350" class="image90" />        
    <button @click="toggleImages35" :class="{ large10: large10 }" class="thirty-fourth-button">Toggle Image 91</button>    
    <!-- Mitral Regurgitation Card -->
    <img v-if="showimage91" src="https://i.imgur.com/7TAhFQP.png" alt="Image 91" height="250" width= "600" class="image91" />
    <!-- Mitral Regurgitation Button -->
    <img v-if="showimage92" src="https://i.imgur.com/2b4U0LB.png" alt="Image 92" height="150" width= "350" class="image92" />  
    <button @click="toggleImages36" :class="{ large11: large11 }" class="thirty-fifth-button">Toggle Image 93</button>    
    <!-- Atrial Flutter Card -->
    <img v-if="showimage93" src="https://i.imgur.com/OYKWGa3.png" alt="Image 93" height="350" width= "650" class="image93" />
    <!-- Atrial Flutter Button -->
    <img v-if="showimage94" src="https://i.imgur.com/PPpKHUm.png" alt="Image 94" height="150" width= "250" class="image94" /> 
    <button @click="toggleImages37" :class="{ large12: large12 }" class="thirty-fixth-button">Toggle Image 95</button>    
    <!-- Atrial Fibrillation Card -->
    <img v-if="showimage95" src="https://i.imgur.com/15yGABM.png" alt="Image 95" height="400" width= "650" class="image95" />
    <!-- Atrial Fibrillation Button -->
    <img v-if="showimage96" src="https://i.imgur.com/TqCFIbF.png" alt="Image 96" height="150" width= "350" class="image96" />     
    <button @click="toggleImages38" :class="{ large13: large13 }" class="thirty-sixth-button">Toggle Image 97</button>    
    <!-- 2 AV Block Card -->
    <img v-if="showimage97" src="https://i.imgur.com/Jz8oPXX.png" alt="Image 97" height="400" width= "650" class="image97" />
    <!-- 2 AV Block Button -->
    <img v-if="showimage98" src="https://i.imgur.com/z8ngb8M.png" alt="Image 98" height="150" width= "300" class="image98" />            
    <button @click="toggleImages39" :class="{ large14: large14 }" class="thirty-seventh-button">Toggle Image 99</button>    
    <!-- Abdominal Aortic Aneurysm Card -->
    <img v-if="showimage99" src="https://i.imgur.com/gPkHKDX.png" alt="Image 99" height="400" width= "850" class="image99" />
    <!-- Abdominal Aortic Aneurysm Button -->
    <img v-if="showimage100" src="https://i.imgur.com/YJ3CeTl.png" alt="Image 100" height="200" width= "300" class="image100" />
    <button @click="toggleImages40" :class="{ large15: large15 }" class="thirty-eigth-button">Toggle Image 101</button>    
    <!-- Premature Ventricular Contraction Card -->
    <img v-if="showimage101" src="https://i.imgur.com/yynwH0Y.png" alt="Image 101" height="400" width= "550" class="image101" />     
    <!-- Premature Ventricular Contraction Button -->
    <img v-if="showimage102" src="https://i.imgur.com/ky5b7Gw.png" alt="Image 102" height="200" width= "300" class="image102" />     
    <button @click="toggleImages41" :class="{ large16: large16 }" class="thirty-ninenth-button">Toggle Image 103</button>    
    <!-- Transposition of the Great Vessels Card -->
    <img v-if="showimage103" src="https://i.imgur.com/yynwH0Y.png" alt="Image 103" height="400" width= "550" class="image103" />       
    <!-- Transposition of the Great Vessels Button -->
    <img v-if="showimage104" src="https://i.imgur.com/w07kW3G.png" alt="Image 104" height="150" width= "450" class="image104" />    
    <button @click="toggleImages42" :class="{ large17: large17 }" class="fortieth-button">Toggle Image 105</button>    
    <!-- Tetrallogy of Fallot Card -->
    <img v-if="showimage105" src="https://i.imgur.com/uv3O0L8.png" alt="Image 105" height="400" width= "650" class="image105" />
    <!-- Tetrallogy of Fallot Button -->
    <img v-if="showimage106" src="https://i.imgur.com/rtqCtQv.png" alt="Image 106" height="150" width= "400" class="image106" />      
    <button @click="toggleImages43" :class="{ large18: large18 }" class="fourty-first-button">Toggle Image 107</button>    
    <!-- Coarctation of the Aorta Card -->
    <img v-if="showimage107" src="https://i.imgur.com/dYbQGMc.png" alt="Image 107" height="400" width= "950" class="image107" />
    <!-- Coarctation of the Aorta Button -->
    <img v-if="showimage108" src="https://i.imgur.com/fJAkcy7.png" alt="Image 108" height="250" width= "400" class="image108" />       
    <button @click="toggleImages44" :class="{ large19: large19 }" class="fourty-second-button">Toggle Image 109</button> 
    <!-- Aortic Dissection Card -->
    <img v-if="showimage109" src="https://i.imgur.com/WsPh3lu.png" alt="Image 109" height="600" width= "550" class="image109" />         
    <!-- Aortic Dissection Button -->
    <img v-if="showimage110" src="https://i.imgur.com/IH72645.png" alt="Image 110" height="150" width= "325" class="image110" />  
    <button @click="toggleImages45" :class="{ large20: large20 }" class="fourty-third-button">Toggle Image 111</button>    
    <!-- Hypertrophic Obstructive Cardiomyopathy Card -->
    <img v-if="showimage111" src="https://i.imgur.com/CXfKuMl.png" alt="Image 111" height="500" width= "750" class="image111" />
    <!-- Hypertrophic Obstructive Cardiomyopathy Button -->
    <img v-if="showimage112" src="https://i.imgur.com/0GoXFRM.png" alt="Image 112" height="150" width= "325" class="image112" />     
    <button @click="toggleImages46" class="forty-fourth-button">Toggle Image 113</button>                     
    <!-- Improve with Rest Phrase -->
    <img v-if="showimage113" src="https://i.imgur.com/ARQFmFN.png" alt="Image 113" height="100" width= "200" class="image113" />    
    <!-- Improve with Rest Button-->
    <img v-if="showimage114" src="https://i.imgur.com/Kce3AsZ.png" alt="Image 114" height="150" width= "150" class="image114" />   
    <button @click="toggleImages47" class="forty-fifth-button">Toggle Image 116</button>                     
    <!-- Emotional Distress Phrase -->
    <img v-if="showimage116" src="https://i.imgur.com/tY3mm5T.png" alt="Image 116" height="100" width= "200" class="image116" />    
    <!-- Emotional Distress Button-->
    <img v-if="showimage117" src="https://i.imgur.com/F7uBtan.png" alt="Image 176" height="150" width= "150" class="image117" />    
    <button @click="toggleImages48" :class="{ large21: large21 }" class="fourty-sixth-button">Toggle Image 119</button>    
    <!-- Stable Angina Card -->
    <img v-if="showimage119" src="https://i.imgur.com/ufwjuCM.png" alt="Image 119" height="400" width= "750" class="image119" />
    <!-- Stable Angina Button -->
    <img v-if="showimage120" src="https://i.imgur.com/89Yvu3b.png" alt="Image 120" height="150" width= "230" class="image120" />     
    <button @click="toggleImages49" :class="{ large22: large22 }" class="fourty-seventh-button">Toggle Image 121</button>    
    <!-- Unstable Angina Card -->
    <img v-if="showimage121" src="https://i.imgur.com/yoedfLg.png" alt="Image 121" height="400" width= "750" class="image121" />
    <!-- Unstable Angina Button -->
    <img v-if="showimage122" src="https://i.imgur.com/AqTJ0GO.png" alt="Image 122" height="150" width= "275" class="image122" />     
    <button @click="toggleImages50" :class="{ large23: large23 }" class="fourty-eigth-button">Toggle Image 123</button>    
    <!-- None ST Eleveated Myocardial Infarction Card -->
    <img v-if="showimage123" src="https://i.imgur.com/BQ93ALj.png" alt="Image 123" height="400" width= "850" class="image123" />
    <!-- None ST Eleveated Myocardial Infarction Button -->
    <img v-if="showimage124" src="https://i.imgur.com/xcVhfJ0.png" alt="Image 124" height="150" width= "325" class="image124" />     
    <button @click="toggleImages51" :class="{ large24: large24 }" class="fourty-ninenth-button">Toggle Image 125</button>    
    <!-- ST Eleveated Myocardial Infarction Card -->
    <img v-if="showimage125" src="https://i.imgur.com/qRNWuzR.png" alt="Image 125" height="400" width= "750" class="image125" />
    <!-- ST Eleveated Myocardial Infarction Button -->
    <img v-if="showimage126" src="https://i.imgur.com/trCdEUR.png" alt="Image 126" height="175" width= "275" class="image126" />     
    <button @click="toggleImages52" :class="{ large25: large25 }" class="fiftieth-button">Toggle Image 127</button>    
    <!-- Takatsubos Disease Card -->
    <img v-if="showimage127" src="https://i.imgur.com/mV0K3ko.png" alt="Image 127" height="400" width= "750" class="image127" />
    <!-- Takatsubos Disease Button -->
    <img v-if="showimage128" src="https://i.imgur.com/q8Q5QcJ.png" alt="Image 128" height="150" width= "325" class="image128" />     
    <!-- Murmur - Hypertrophic Obstructive Cardiomyopathy -->
    <img v-if="showimage129" src="https://i.imgur.com/1wdcIsR.png" alt="Image 129" height="400" width= "20" class="image129" />      
    <!-- Palpitations - Hypertrophic Obstructive Cardiomyopathy -->
    <img v-if="showimage130" src="https://i.imgur.com/1vvSG3Z.png" alt="Image 130" height="600" width= "350" class="image130" />        
    <!-- Murmur - Low Pitch Holosystolic -->
    <img v-if="showimage131" src="https://i.imgur.com/QK5J5H2.png" alt="Image 131" height="350" width= "250" class="image131" />      
    <!-- Low Pitch Holosystolic - Mitral Regurgitation -->
    <img v-if="showimage132" src="https://i.imgur.com/GNqm2Qp.png" alt="Image 132" height="300" width= "200" class="image132" />    
    <!-- Palpitation - Tachycardia -->
    <img v-if="showimage133" src="https://i.imgur.com/ndtBwyi.png" alt="Image 133" height="450" width= "100" class="image133" />       
    <!-- Tachycardia - Atrial Flutter -->
    <img v-if="showimage134" src="https://i.imgur.com/9hnbtjG.png" alt="Image 134" height="300" width= "80" class="image134" />   
    <!-- Tachycardia - Atrial Fibrillation -->
    <img v-if="showimage135" src="https://i.imgur.com/8iZKjfx.png" alt="Image 135" height="350" width= "275" class="image135" /> 
    <!-- Palpitation - Bradycardia -->
    <img v-if="showimage136" src="https://i.imgur.com/MJWmQnt.png" alt="Image 136" height="300" width= "300" class="image136" />      
    <!-- Bradycardia - 2 AV Block -->
    <img v-if="showimage137" src="https://i.imgur.com/Jk5J5nT.png" alt="Image 137" height="300" width= "300" class="image137" />    
    <!-- Syncope - Back Pain -->
    <img v-if="showimage138" src="https://i.imgur.com/YnowZAx.png" alt="Image 138" height="300" width= "300" class="image138" />   
    <!-- Back Pain - Aortic Abdominal Aneurysm -->
    <img v-if="showimage139" src="https://i.imgur.com/a1bDqpu.png" alt="Image 139" height="300" width= "350" class="image139" />  
    <!-- Syncope - Asymptomatic Baseline -->
    <img v-if="showimage140" src="https://i.imgur.com/11slhS1.png" alt="Image 140" height="125" width= "400" class="image140" />    
    <!-- Asymptomatic Baseline - Premature Ventricular Contraction -->
    <img v-if="showimage141" src="https://i.imgur.com/H7qo5fe.png" alt="Image 141" height="250" width= "450" class="image141" />          
    <!-- Congenital - Blue Cyanosis -->
    <img v-if="showimage142" src="https://i.imgur.com/betxp92.png" alt="Image 142" height="20" width= "500" class="image142" />        
    <!-- Blue Cyanosis - Transposition of the Great Vessels -->
    <img v-if="showimage143" src="https://i.imgur.com/idqdrJX.png" alt="Image 143" height="250" width= "450" class="image143" />       
    <!-- Blue Cyanosis - Tetrallogy of Fallot -->
    <img v-if="showimage144" src="https://i.imgur.com/hDr6JYJ.png" alt="Image 144" height="180" width= "450" class="image144" />  
    <!-- Low Limb - Coarctation of the Aorta -->
    <img v-if="showimage145" src="https://i.imgur.com/CYjpmd9.png" alt="Image 145" height="225" width= "500" class="image145" />           
    <!-- Lower Limb - Aortic Dissection -->
    <img v-if="showimage146" src="https://i.imgur.com/OZemUeo.png" alt="Image 146" height="450" width= "350" class="image146" />  
    <!-- Chest Pain - Tearing Chest Pain -->
    <img v-if="showimage147" src="https://i.imgur.com/QxaTQ9T.png" alt="Image 147" height="350" width= "325" class="image147" />         
    <!-- Tearing Chest Pain - Aortic Dissection -->
    <img v-if="showimage148" src="https://i.imgur.com/uP3wbXs.png" alt="Image 148" height="25" width= "275" class="image148" />  
    <!-- Chest Pain - Substernal Chest Pain -->
    <img v-if="showimage149" src="https://i.imgur.com/yDeb6qe.png" alt="Image 149" height= "400" width= "20" class="image149" />         
    <!-- Chest Pain - Sharp Chest Pain -->
    <img v-if="showimage150" src="https://i.imgur.com/5Qvf6Pd.png" alt="Image 150" height="350" width= "325" class="image150" />     
    <!-- Fever - Chagas -->
    <img v-if="showimage151" src="https://i.imgur.com/VFJaUgH.png" alt="Image 151" height="250" width= "150" class="image151" /> 
    <!-- Fever - Infective Endocarditis -->
    <img v-if="showimage152" src="https://i.imgur.com/uP3wbXs.png" alt="Image 152" height="25" width= "200" class="image152" />   
    <!-- Weight Loss - Atrial Myxoma -->
    <img v-if="showimage153" src="https://i.imgur.com/uP3wbXs.png" alt="Image 153" height="25" width= "300" class="image153" />  
    <!-- Weight Loss - Infective Endocarditis -->
    <img v-if="showimage154" src="https://i.imgur.com/Qri5tvB.png" alt="Image 154" height="225" width= "200" class="image154" />      
    <!-- Peripheral Edema - Red Lower Limb -->
    <img v-if="showimage155" src="https://i.imgur.com/27yZsJr.png" alt="Image 155" height="125" width= "400" class="image155" />  
    <!-- Red Lower Limb - Deep Venous Thrombosis -->
    <img v-if="showimage156" src="https://i.imgur.com/CpH4n7A.png" alt="Image 156" height="150" width= "275" class="image156" />     
    <!-- Peripheral Edema - CREAM -->
    <img v-if="showimage157" src="https://i.imgur.com/uyZYWEx.png" alt="Image 157" height="200" width= "425" class="image157" />      
    <!-- CREAM - Kawasakis Disease -->
    <img v-if="showimage158" src="https://i.imgur.com/TxERLtz.png" alt="Image 158" height="275" width= "275" class="image158" />       
    <!-- Jugular Venous Distention - Decreased Heart Sound -->
    <img v-if="showimage159" src="https://i.imgur.com/ik3R5yz.png" alt="Image 159" height="325" width= "275" class="image159" />     
    <!-- Decreased Heart Sound - Hypotension -->
    <img v-if="showimage160" src="https://i.imgur.com/ttNKUPM.png" alt="Image 160" height="325" width= "275" class="image160" />   
    <!-- Hypotension - Pericardial Effusion -->
    <img v-if="showimage161" src="https://i.imgur.com/r7sDFz1.png" alt="Image 161" height="500" width= "250" class="image161" />     
    <!-- Hypotension - Cardiac Tamponade -->
    <img v-if="showimage162" src="https://i.imgur.com/E36FZvS.png" alt="Image 162" height="275" width= "625" class="image162" /> 
    <!-- Substernal Chest Pain - Improve with Rest -->
    <img v-if="showimage163" src="https://i.imgur.com/kvxmHuE.png" alt="Image 163" height="450" width= "20" class="image163" />     
    <!-- Improve with Rest - None ST Elevated Myocardial Infarction -->
    <img v-if="showimage164" src="https://i.imgur.com/kvxmHuE.png" alt="Image 164" height="400" width= "20" class="image164" /> 
    <!-- Sharp Chest Pain - Uremic Pericarditis -->
    <img v-if="showimage165" src="https://i.imgur.com/lGLhfOn.png" alt="Image 165" height="300" width= "400" class="image165" />     
    <!-- Singularity 1 - Emotional Distress -->
    <img v-if="showimage166" src="https://i.imgur.com/9sFsovq.png" alt="Image 166" height="20" width= "500" class="image166" />  
    <!-- Emotional Distress - Takatsubos Disease -->
    <img v-if="showimage167" src="https://i.imgur.com/betxp92.png" alt="Image 167" height="20" width= "300" class="image167" /> 
    <!-- Singularity 1 - Stable Angina -->
    <img v-if="showimage168" src="https://i.imgur.com/9sFsovq.png" alt="Image 168" height="20" width= "425" class="image168" /> 
    <!-- Singularity 1 - Unstable Angina -->
    <img v-if="showimage169" src="https://i.imgur.com/9byPES1.png" alt="Image 169" height="175" width= "225" class="image169" />    
    <!-- Singularity 1 - ST Elevated Myocardial Infarction -->
    <img v-if="showimage170" src="https://i.imgur.com/w6cl8qx.png" alt="Image 170" height="175" width= "225" class="image170" />                                                                                                                               
  </div>
</template>

<script>
export default {
  data() {
    return {
      showimage1: false, // initialize Cardio Fundamentals with a value of true
      showimage2: true, // initialize Heart Button with a value of true
      showimage3: false, // initialize  with a value of true
      showimage4: true, // initialize Palpitation Button with a value of true
      showimage5: true, // initialize  with a value of true
      showimage6: false, // initialize  with a value of true
      showimage7: true, // initialize Chest Pain Button with a value of true
      showimage8: true, // initialize  with a value of true 
      showimage9: false, // initialize  with a value of true
      showimage10: true, // initialize Congenital Button with a value of true
      showimage11: true, // initialize  with a value of true           
      showimage12: false, // initialize  with a value of true
      showimage13: true, // initialize Fever Button with a value of true
      showimage14: true, // initialize  with a value of true
      showimage15: false, // initialize  with a value of true
      showimage16: true, // initialize Jugular Venous Distention Button with a value of true
      showimage17: true, // initialize  with a value of true
      showimage18: false, // initialize  with a value of true
      showimage19: true, // initialize Lower Limb Low Blood Pressure Button with a value of true
      showimage20: true, // initialize  with a value of true
      showimage21: false, // initialize  with a value of true
      showimage22: true, // initialize Murmur Button with a value of true
      showimage23: true, // initialize  with a value of true
      showimage24: false, // initialize  with a value of true
      showimage25: true, // initialize Peripheral Edema Button with a value of true
      showimage26: true, // initialize  with a value of true
      showimage27: false, // initialize  with a value of true
      showimage28: true, // initialize Syncope Button with a value of true
      showimage29: true, // initialize  with a value of true
      showimage30: false, // initialize  with a value of true
      showimage31: true, // initialize Weight Loss Button with a value of true
      showimage32: true, // initialize showimage32 with a value of true
      showimage33: false, // initialize Substernal Chest Pain Button with a value of true
      showimage34: true, // 
      showimage35: true, // 
      showimage39: false, // initialize Cyanosis Button with a value of true
      showimage40: true, // 
      showimage41: true, // 
      showimage42: false, // initialize Tearing Chest Pain Button with a value of true
      showimage43: true, // 
      showimage44: true, // 
      showimage45: false, // initialize Sharp Chest Pain Button with a value of true
      showimage46: true, // 
      showimage47: true, // 
      showimage48: false, // initialize Low Pitch Holosystolic Button with a value of true
      showimage49: true, // 
      showimage50: true, // 
      showimage51: false, // initialize CREAM Button with a value of true
      showimage52: true, // 
      showimage53: true, // 
      showimage54: false, // initialize Red LL Button with a value of true
      showimage55: true, // 
      showimage56: true, // 
      showimage57: false, // initialize Decreased Heart Sound Button with a value of true
      showimage58: true, // 
      showimage59: true, //  
      showimage60: false, // initialize Tachycardia Button with a value of true
      showimage61: true, // 
      showimage62: true, //        
      showimage63: false, // initialize Bradycardia Button with a value of true
      showimage64: true, // 
      showimage65: true, // 
      showimage66: false, // initialize Back Pain Button with a value of true
      showimage67: true, // 
      showimage68: true, // 
      showimage69: false, // initialize Baseline Asymptomatic Button with a value of true
      showimage70: true, // 
      showimage71: true, // 
      showimage72: false, // initialize Baseline Asymptomatic Button with a value of true
      showimage73: true, // 
      showimage74: true, // 
      showimage75: false, // initialize Uermic Pericarditis Card with a value of true
      showimage76: true, // 
      showimage77: false, // initialize Chagas Disease Card with a value of true
      showimage78: true, // 
      showimage79: false, // initialize Infective Endocarditis Card with a value of true
      showimage80: true, // 
      showimage81: false, // initialize Atrial Myxoma Card with a value of true
      showimage82: true, //
      showimage83: false, // initialize Deep Venous Thrombosis Card with a value of true
      showimage84: true, //
      showimage85: false, // initialize Kawasakis Disease Card with a value of true
      showimage86: true, //
      showimage87: false, // initialize Cardiac Tamponade Card with a value of true
      showimage88: true, //
      showimage89: false, // initialize Pericardial Effusion Card with a value of true
      showimage90: true, //
      showimage91: false, // initialize Mitral Regurgitation Card with a value of true
      showimage92: true, //
      showimage93: false, // initialize Atrial Flutter Card with a value of true
      showimage94: true, //
      showimage95: false, // initialize Atrial Fibrillation Card with a value of true
      showimage96: true, //
      showimage97: false, // initialize 2 AV Block Card with a value of true
      showimage98: true, //
      showimage99: false, // initialize Abdominal Aortic Aneurysm Card with a value of true
      showimage100: true, //
      showimage101: false, // initialize Abdominal Premature Ventricular Contraction Card with a value of true
      showimage102: true, //
      showimage103: false, // initialize Abdominal Premature Ventricular Contraction Card with a value of true
      showimage104: true, //
      showimage105: false, // initialize Tetrallogy of Fallot Card with a value of true
      showimage106: true, //
      showimage107: false, // initialize Coarctation of the Aorta Card with a value of true
      showimage108: true, //
      showimage109: false, // initialize Aortic Dissection Card with a value of true
      showimage110: true, //
      showimage111: false, // initialize Hypertrophic Obstructive Cardiomyopathy Card with a value of true
      showimage112: true, //
      showimage113: false, // initialize Improve with Rest Button with a value of true
      showimage114: true, // 
      showimage115: true, // 
      showimage116: false, // initialize Emotional Distress Button with a value of true
      showimage117: true, // 
      showimage118: true, // 
      showimage119: false, // initialize Stable Angina Card with a value of true
      showimage120: true, //
      showimage121: false, // initialize Unstable Angina Card with a value of true
      showimage122: true, //
      showimage123: false, // initialize None ST Elevated Myocardial Infarction Card with a value of true
      showimage124: true, //
      showimage125: false, // initialize ST Elevated Myocardial Infarction Card with a value of true
      showimage126: true, //
      showimage127: false, // initialize Takatsubos Disease Card with a value of true
      showimage128: true, //
      showimage129: true, //
      showimage130: true, //
      showimage131: true, //
      showimage132: true, //
      showimage133: true, //
      showimage134: true, //
      showimage135: true, //
      showimage136: true, //
      showimage137: true, //
      showimage138: true, //
      showimage139: true, //
      showimage140: true, //
      showimage141: true, //
      showimage142: true, //
      showimage143: true, //
      showimage144: true, //
      showimage145: true, //
      showimage146: true, //
      showimage147: true, //
      showimage148: true, //
      showimage149: true, //
      showimage150: true, //
      showimage151: true, //
      showimage152: true, //
      showimage153: true, //
      showimage154: true, //
      showimage155: true, //
      showimage156: true, //
      showimage157: true, //
      showimage158: true, //
      showimage159: true, //
      showimage160: true, //
      showimage161: true, //
      showimage162: true, //
      showimage163: true, //
      showimage164: true, //
      showimage165: true, //
      showimage166: true, //
      showimage167: true, //
      showimage168: true, //
      showimage169: true, //
      showimage170: true, //
      showimage171: true, //
      large: false, // 
      large2: false, // 
      large3: false, //   
      large4: false, //  
      large5: false, //   
      large6: false, //   
      large7: false, //   
      large8: false, //   
      large9: false, //   
      large10: false, //   
      large11: false, //   
      large12: false, //   
      large13: false, //   
      large14: false, //   
      large15: false, //   
      large16: false, //   
      large17: false, //   
      large18: false, //   
      large19: false, //    
      large20: false, //   
      large21: false, // 
      large22: false, // 
      large23: false, // 
      large24: false, // 
      large25: false, // 
    }
  },
  methods: {
    toggleLists() {
      this.showimage1 = !this.showimage1;
      this.showimage2 = !this.showimage2; // toggle the value of showimage2
      this.large = !this.large // toggle the value of large
    },
    toggleImages3() {
      this.showimage3 = !this.showimage3; // toggle the value of Palpitation Phrase
    },
    toggleImages4() {
      this.showimage6 = !this.showimage6; // toggle the value of Chest Pain Phrase
    },
    toggleImages5() {
      this.showimage9 = !this.showimage9; // toggle the value of Congenital Phrase
    },
    toggleImages6() {
      this.showimage12 = !this.showimage12; // toggle the value of Fever Phrase
    },
    toggleImages7() {
      this.showimage15 = !this.showimage15; // toggle the value of Jugular Venous Distention Phrase
    },
    toggleImages8() {
      this.showimage18 = !this.showimage18; // toggle the value of Lower Limb Low Blood Pressure Phrase
    },
    toggleImages9() {
      this.showimage21 = !this.showimage21; // toggle the value of Murmur Phrase
    },
    toggleImages10() {
      this.showimage24 = !this.showimage24; // toggle the value of Peripheral Edema Phrase
    },
    toggleImages11() {
      this.showimage27 = !this.showimage27; // toggle the value of Syncope Phrase
    },
    toggleImages12() {
      this.showimage30 = !this.showimage30; // toggle the value of Weight Loss Phrase
    },
    toggleImages13() {
      this.showimage33 = !this.showimage33; // toggle the value of Substernal Chest Pain Phrase
    },
    toggleImages15() {
      this.showimage39 = !this.showimage39; // toggle the value of Blue Cyanosis Phrase
    },
    toggleImages16() {
      this.showimage42 = !this.showimage42; // toggle the value of Tearing Chest Pain Phrase
    },
    toggleImages17() {
      this.showimage45 = !this.showimage45; // toggle the value of Sharp Chest Pain Phrase
    },  
    toggleImages18() {
      this.showimage48 = !this.showimage48; // toggle the value of Low Pitch Holosystolic Phrase
    },  
    toggleImages19() {
      this.showimage51 = !this.showimage51; // toggle the value of CREAM Phrase
    },  
    toggleImages20() {
      this.showimage54 = !this.showimage54; // toggle the value of Red LL Phrase
    },  
    toggleImages21() {
      this.showimage57 = !this.showimage57; // toggle the value of Decreased Heart Sound Phrase
    },    
    toggleImages22() {
      this.showimage60 = !this.showimage60; // toggle the value of Tachycardia Phrase
    },   
    toggleImages23() {
      this.showimage63 = !this.showimage63; // toggle the value of Bradycardia Phrase
    },   
    toggleImages24() {
      this.showimage66 = !this.showimage66; // toggle the value of Back Pain Phrase
    },   
    toggleImages25() {
      this.showimage69 = !this.showimage69; // toggle the value of Baseline Asymptomatic Phrase
    },   
    toggleImages26() {
      this.showimage72 = !this.showimage72; // toggle the value of Hypotension Phrase
    },   
    toggleImages27() {
      this.showimage75 = !this.showimage75; // toggle the value of Uremic Pericarditis Phrase
      this.showimage76 = !this.showimage76; 
      this.large2 = !this.large2; // toggle the value of large
    },   
    toggleImages28() {
      this.showimage77 = !this.showimage77; // toggle the value of Chagas Disease Phrase
      this.showimage78 = !this.showimage78; 
      this.large3 = !this.large3; // toggle the value of large
    },  
    toggleImages29() {
      this.showimage79 = !this.showimage79; // toggle the value of Infective Endocarditis Phrase
      this.showimage80 = !this.showimage80; 
      this.large4 = !this.large4; // toggle the value of large
    },  
    toggleImages30() {
      this.showimage81 = !this.showimage81; // toggle the value of Atrial Myxoma Phrase
      this.showimage82 = !this.showimage82; 
      this.large5 = !this.large5; // toggle the value of large
    },  
    toggleImages31() {
      this.showimage83 = !this.showimage83; // toggle the value of Deep Venous Thrombosis Phrase
      this.showimage84 = !this.showimage84; 
      this.large6 = !this.large6; // toggle the value of large
    },  
    toggleImages32() {
      this.showimage85 = !this.showimage85; // toggle the value of Kawasakis Disease Phrase
      this.showimage86 = !this.showimage86; 
      this.large7 = !this.large7; // toggle the value of large
    },  
    toggleImages33() {
      this.showimage87 = !this.showimage87; // toggle the value of Cardiac Tamponade Phrase
      this.showimage88 = !this.showimage88; 
      this.large8 = !this.large8; // toggle the value of large
    },  
    toggleImages34() {
      this.showimage89 = !this.showimage89; // toggle the value of Pericardial Effusion Phrase
      this.showimage90 = !this.showimage90; 
      this.large9 = !this.large9; // toggle the value of large
    },  
    toggleImages35() {
      this.showimage91 = !this.showimage91; // toggle the value of Mitral Regurgitation Phrase
      this.showimage92 = !this.showimage92; 
      this.large10 = !this.large10; // toggle the value of large
    },  
    toggleImages36() {
      this.showimage93 = !this.showimage93; // toggle the Atrial Flutter Phrase
      this.showimage94 = !this.showimage94; 
      this.large11 = !this.large11; // toggle the value of large
    }, 
    toggleImages37() {
      this.showimage95 = !this.showimage95; // toggle the value of Atrial Fibrillation Phrase
      this.showimage96 = !this.showimage96; 
      this.large12 = !this.large12; // toggle the value of large
    }, 
    toggleImages38() {
      this.showimage97 = !this.showimage97; // toggle the value of 2 AV Block Phrase
      this.showimage98 = !this.showimage98; 
      this.large13 = !this.large13; // toggle the value of large
    }, 
    toggleImages39() {
      this.showimage99 = !this.showimage99; // toggle the value of Abdominal Aortic Aneurysm Phrase
      this.showimage100 = !this.showimage100; 
      this.large14 = !this.large14; // toggle the value of large
    }, 
    toggleImages40() {
      this.showimage101 = !this.showimage101; // toggle the value of Premature Ventricular Contraction Phrase
      this.showimage102 = !this.showimage102; 
      this.large15 = !this.large15; // toggle the value of large
    }, 
    toggleImages41() {
      this.showimage103 = !this.showimage103; // toggle the value of Transposition of the Great Vessels Phrase
      this.showimage104 = !this.showimage104; 
      this.large16 = !this.large16; // toggle the value of large
    }, 
    toggleImages42() {
      this.showimage105 = !this.showimage105; // toggle the value of Tetrallogy of Fallot Phrase
      this.showimage106 = !this.showimage106; 
      this.large17 = !this.large17; // toggle the value of large
    }, 
    toggleImages43() {
      this.showimage107 = !this.showimage107; // toggle the value of Coarctation of the Aorta Phrase
      this.showimage108 = !this.showimage108; 
      this.large18 = !this.large18; // toggle the value of large
    }, 
    toggleImages44() {
      this.showimage109 = !this.showimage109; // toggle the value of Aortic Dissection Phrase
      this.showimage110 = !this.showimage110; 
      this.large19 = !this.large19; // toggle the value of large
    }, 
    toggleImages45() {
      this.showimage111 = !this.showimage111; // toggle the value of Hypertrophic Obstructive Cardiomyopathy Phrase
      this.showimage112 = !this.showimage112; 
      this.large20 = !this.large20; // toggle the value of large
    }, 
    toggleImages46() {
      this.showimage113 = !this.showimage113; // toggle the value of Improve with Rest Phrase
    },   
    toggleImages47() {
      this.showimage116 = !this.showimage116; // toggle the value of Emotional Distress Phrase
    },   
    toggleImages48() {
      this.showimage119 = !this.showimage119; // toggle the value of Stable Angina Phrase
      this.showimage120 = !this.showimage120; 
      this.large21 = !this.large21; // toggle the value of large
    }, 
    toggleImages49() {
      this.showimage121 = !this.showimage121; // toggle the value of Unstable Angina Phrase
      this.showimage122 = !this.showimage122; 
      this.large22 = !this.large22; // toggle the value of large
    }, 
    toggleImages50() {
      this.showimage123 = !this.showimage123; // toggle the value of None ST Elevated Myocardial Infarction Phrase
      this.showimage124 = !this.showimage124; 
      this.large23 = !this.large23; // toggle the value of large
    }, 
    toggleImages51() {
      this.showimage125 = !this.showimage125; // toggle the value of ST Elevated Myocardial Infarction Phrase
      this.showimage126 = !this.showimage126; 
      this.large24 = !this.large24; // toggle the value of large
    }, 
    toggleImages52() {
      this.showimage127 = !this.showimage127; // toggle the value of Takatsubos Disease Phrase
      this.showimage128 = !this.showimage128; 
      this.large25 = !this.large25; // toggle the value of large
    }, 
  },
  
  mounted() {
    // Scroll to the coordinates (Xpx, Ypx)
    window.scrollTo(3475, 3950);
  }
}
</script>


<style>
  /* remove bullet points from all lists */
  ul {
    list-style-type: none;
  }

  /* styles for the body */
  body {
    background-color: #000733;
    font-family: Arial;
    color: #F0F1F9;
    width: 9000px;
    height: 9000px;
    margin: 100px;
  }

  /* styles for the button */
  button {
    position: absolute;
    top: 4400px;
    left: 4350px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1; /* this will position the button behind the images */
    opacity: 0;
  }

  /* styles for the button when it's in the large state */
  button.large {
    top: 4075px;
    left: 4100px;
    height: 800px; /* this will make the button twice as big as the default size */
    width: 625px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }  

  /* styles for the Palpitation button */
  .second-button {
    position: absolute;
    top: 4862px;
    left: 4040px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.7; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Chest Pain button */
  .third-button {
    position: absolute;
    top: 3802px;
    left: 4347px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Congenital button */
  .fourth-button {
    position: absolute;
    top: 4402px;
    left: 3649px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Fever button */
  .fifth-button {
    position: absolute;
    top: 3987px;
    left: 4837px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Jugular Venous Distention button */
  .sixth-button {
    position: absolute;
    top: 4864px;
    left: 4687px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Lower Limb Low Blood Pressure button */
  .seventh-button {
    position: absolute;
    top: 3987px;
    left: 3889px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Murmur button */
  .eighth-button {
    position: absolute;
    top: 5002px;
    left: 4347px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Peripheral Edema button */
  .ninth-button {
    position: absolute;
    top: 4662px;
    left: 4887px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Syncope button */
  .tenth-button {
    position: absolute;
    top: 4662px;
    left: 3739px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Weight Loss button */
  .tenth-button {
    position: absolute;
    top: 4662px;
    left: 3737px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }  

  /* styles for the Weight Loss button */
  .eleventh-button {
    position: absolute;
    top: 4402px;
    left: 5047px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  } 

  /* styles for the Substernal Chest Pain button */
  .twelfth-button {
    position: absolute;
    top: 3203px;
    left: 4347px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }     

  /* styles for the Cyanosis button */
  .fourteenth-button {
    position: absolute;
    top: 4400px;
    left: 2945px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }     

  /* styles for the Tearing Chest Pain button */
  .fifteenth-button {
    position: absolute;
    top: 3300px;
    left: 3890px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }    

  /* styles for the Sharp Chest Pain button */
  .sixteenth-button {
    position: absolute;
    top: 3305px;
    left: 4790px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }      

  /* styles for the Low Pitch Holosystolic button */
  .seventeenth-button {
    position: absolute;
    top: 5540px;
    left: 4740px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }      

  /* styles for the CREAM button */
  .eightteenth-button {
    position: absolute;
    top: 5103px;
    left: 5288px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }      

  /* styles for the Red LL button */
  .nineteenth-button {
    position: absolute;
    top: 4800px;
    left: 5485px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the Decreased Heart Sound button */
  .twentieth-button {
    position: absolute;
    top: 5335px;
    left: 5035px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }     

    /* styles for the Tachycardia button */
    .twenty-first-button {
    position: absolute;
    top: 5535px;
    left: 3935px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  } 

    /* styles for the Bradycardia button */
    .twenty-second-button {
    position: absolute;
    top: 5338px;
    left: 3585px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }   
  
    /* styles for the Back Pain button */
    .twenty-third-button {
    position: absolute;
    top: 5105px;
    left: 3285px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }     

    /* styles for the Baseline Asymptmatic button */
    .twenty-fourth-button {
    position: absolute;
    top: 4805px;
    left: 3090px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

    /* styles for the Hypotension button */
    .twenty-fifth-button {
    position: absolute;
    top: 5775px;
    left: 5475px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }     

    /* styles for the Uremic Pericarditis button */
    .twenty-sixth-button {
    position: absolute;
    top: 2845px;
    left: 5168px;
    height: 75px; /* this will make the button bigger */
    width: 165px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large2 {
    top: 2155px;
    left: 5090px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 650px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }  

    /* styles for the Chagas Disease button */
    .twenty-seventh-button {
    position: absolute;
    top: 3590px;
    left: 5070px;
    height: 75px; /* this will make the button bigger */
    width: 140px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large3 {
    top: 3550px;
    left: 5000px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 700px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }   

    /* styles for the Infective Endocarditis button */
    .twenty-eighth-button {
    position: absolute;
    top: 3985px;
    left: 5288px;
    height: 78px; /* this will make the button bigger */
    width: 175px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large4 {
    top: 3950px;
    left: 5200px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 550px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }   

   /* styles for the Atrial Myxoma button */
   .twenty-ninenth-button {
    position: absolute;
    top: 4400px;
    left: 5572px;
    height: 75px; /* this will make the button bigger */
    width: 128px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large5 {
    top: 4365px;
    left: 5510px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 850px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }     

   /* styles for the Deep Venous Thrombosis button */
   .thirtieth-button {
    position: absolute;
    top: 5000px;
    left: 6000px;
    height: 78px; /* this will make the button bigger */
    width: 190px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large6 {
    top: 4965px;
    left: 5910px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 850px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }     

   /* styles for the Kawasakis Disease button */
   .thirty-first-button {
    position: absolute;
    top: 5440px;
    left: 5725px;
    height: 78px; /* this will make the button bigger */
    width: 150px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large7 {
    top: 5400px;
    left: 5650px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 550px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }  

   /* styles for the Cardiac Tamponade button */
   .thirty-second-button {
    position: absolute;
    top: 6140px;
    left: 6140px;
    height: 78px; /* this will make the button bigger */
    width: 178px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large8 {
    top: 6100px;
    left: 6050px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 625px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }       

   /* styles for the Pericardial Effusion button */
   .thirty-third-button {
    position: absolute;
    top: 6440px;
    left: 5635px;
    height: 78px; /* this will make the button bigger */
    width: 175px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large9 {
    top: 6400px;
    left: 5550px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 625px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }      

   /* styles for the Mitral Regurgitation button */
   .thirty-fourth-button {
    position: absolute;
    top: 6035px;
    left: 4940px;
    height: 78px; /* this will make the button bigger */
    width: 175px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large10 {
    top: 6000px;
    left: 4850px;
    height: 250px; /* this will make the button twice as big as the default size */
    width: 600px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }       

   /* styles for the Atrial Flutter button */
   .thirty-fifth-button {
    position: absolute;
    top: 6038px;
    left: 4012px;
    height: 78px; /* this will make the button bigger */
    width: 125px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large11 {
    top: 6000px;
    left: 3950px;
    height: 350px; /* this will make the button twice as big as the default size */
    width: 650px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }     

   /* styles for the Atrial Fibrillation button */
   .thirty-fixth-button {
    position: absolute;
    top: 6040px;
    left: 3535px;
    height: 78px; /* this will make the button bigger */
    width: 175px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large12 {
    top: 6000px;
    left: 3450px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 550px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }       

   /* styles for the 2 AV Block button */
   .thirty-sixth-button {
    position: absolute;
    top: 5833px;
    left: 3120px;
    height: 78px; /* this will make the button bigger */
    width: 155px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large13 {
    top: 5800px;
    left: 3050px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 550px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }       

   /* styles for the Abdominal Aortic Aneurysm button */
   .thirty-seventh-button {
    position: absolute;
    top: 5552px;
    left: 2725px;
    height: 100px; /* this will make the button bigger */
    width: 155px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large14 {
    top: 5500px;
    left: 2650px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 850px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }         

   /* styles for the Premature Ventricular Contraction button */
   .thirty-eigth-button {
    position: absolute;
    top: 5150px;
    left: 2325px;
    height: 100px; /* this will make the button bigger */
    width: 148px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large15 {
    top: 5100px;
    left: 2250px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 550px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }      

   /* styles for the Transposition of the Great Vessels button */
   .thirty-ninenth-button {
    position: absolute;
    top: 4640px;
    left: 2063px;
    height: 80px; /* this will make the button bigger */
    width: 225px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large16 {
    top: 4600px;
    left: 1950px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 5500px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }        

   /* styles for the Tetrallogy of Fallot button */
   .fortieth-button {
    position: absolute;
    top: 4238px;
    left: 2078px;
    height: 75px; /* this will make the button bigger */
    width: 202px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large17 {
    top: 4200px;
    left: 1980px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 550px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }     

   /* styles for the Coarctation of the Aorta button */
   .fourty-first-button {
    position: absolute;
    top: 3760px;
    left: 2980px;
    height: 128px; /* this will make the button bigger */
    width: 202px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large18 {
    top: 3700px;
    left: 2880px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 950px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }       

   /* styles for the Aortic Dissection button */
   .fourty-second-button {
    position: absolute;
    top: 3337px;
    left: 3260px;
    height: 75px; /* this will make the button bigger */
    width: 165px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large19 {
    top: 3300px;
    left: 3180px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 950px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }     

   /* styles for the Hypertrophic Obstructive Cardiomyopathy button */
   .fourty-third-button {
    position: absolute;
    top: 5602px;
    left: 4323px;
    height: 75px; /* this will make the button bigger */
    width: 165px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large20 {
    top: 5565px;
    left: 4240px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 750px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }      

  /* styles for the Improve with Rest button */
  .forty-fourth-button {
    position: absolute;
    top: 2543px;
    left: 4338px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }   

  /* styles for the Emotional Distress button */
  .forty-fifth-button {
    position: absolute;
    top: 2543px;
    left: 5038px;
    height: 75px; /* this will make the button bigger */
    width: 75px; /* this will make the button bigger */
    border-radius: 50% 50%; /* this will create a more rounded shape */
    transform: scale(2); /* this will make the button 1.5 times bigger */
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }   
  
   /* styles for the Stable Angina button */
   .fourty-sixth-button {
    position: absolute;
    top: 2537px;
    left: 3657px;
    height: 78px; /* this will make the button bigger */
    width: 115px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large21 {
    top: 2503px;
    left: 3600px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 750px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }   
  
   /* styles for the Unstable Angina button */
   .fourty-seventh-button {
    position: absolute;
    top: 2188px;
    left: 3870px;
    height: 75px; /* this will make the button bigger */
    width: 138px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 00;
  }       

  /* styles for the button when it's in the large state */
  button.large22 {
    top: 2150px;
    left: 3800px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 7500px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }   
  
   /* styles for the None ST Elevated Myocardial Infarction button */
   .fourty-eigth-button {
    position: absolute;
    top: 1942px;
    left: 4300px;
    height: 75px; /* this will make the button bigger */
    width: 165px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large23 {
    top: 1903px;
    left: 4220px;
    height: 200px; /* this will make the button twice as big as the default size */
    width: 425px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }   
  
   /* styles for the ST Elevated Myocardial Infarction button */
   .fourty-ninenth-button {
    position: absolute;
    top: 2195px;
    left: 4765px; 
    height: 90px; /* this will make the button bigger */
    width: 140px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large24 {
    top: 2150px;
    left: 4700px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 7500px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }   
  
   /* styles for the Takatsubos Disease button */
   .fiftieth-button {
    position: absolute;
    top: 2543px;
    left: 5578px;
    height: 75px; /* this will make the button bigger */
    width: 165px; /* this will make the button bigger */
    border-radius: 0;
    z-index: 1.5; /* this will position the button behind the images */
    opacity: 0;
  }       

  /* styles for the button when it's in the large state */
  button.large25 {
    top: 2502px;
    left: 5500px;
    height: 400px; /* this will make the button twice as big as the default size */
    width: 750px; /* this will make the button twice as big as the default size */
    transform: scale(1); /* this will make the button the same size as the default size */
    border-radius: 0; /* this will remove the rounded corners and make the button a square */
  }     

  /* styles for Cardiovascular Fundamentals */
  img.image1 {
    top: 4075px;
    left: 4100px;
    position: absolute;
    z-index: -1;
  }

  /* styles for Heart Button */
  img.image2 {
    top: 4365px;
    left: 4310px;
    position: absolute;
    z-index: -1;
  }

  /* styles for Palpitation Phrase */
  img.image3 {
  top: 4995px;
  left: 3925px;
  position: absolute;
  z-index: -.5;
  }

  /* styles for Palpitation Button */
  img.image4 {
  top: 4825px;
  left: 4000px;
  position: absolute;
  z-index: -2;
  }

  /* styles for Heart - Palpitation */
  /* Transform skew can help with rotation and tilting of the line */
  img.image5 {
  top: 4525px;
  left: 4075px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Chest Pain Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image6 {
  top: 3925px;
  left: 4275px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Chest Pain Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image7 {
  top: 3765px;
  left: 4310px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart - Chest Pain */
  /* Transform skew can help with rotation and tilting of the line */
  img.image8 {
  top: 3935px;
  left: 4375px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Congenital Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image9 {
  top: 4530px;
  left: 3525px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Congenital Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image10 {
  top: 4365px;
  left: 3610px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart - Congenital */
  /* Transform skew can help with rotation and tilting of the line */
  img.image11 {
  top: 4425px;
  left: 3800px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Fever Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image12 {
  top: 4110px;
  left: 4800px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Fever Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image13 {
  top: 3950px;
  left: 4800px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart Fever */
  /* Transform skew can help with rotation and tilting of the line */
  img.image14 {
  top: 4090px;
  left: 4450px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Jugular Venous Distention Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image15 {
  top: 4990px;
  left: 4575px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Jugular Venous Distention Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image16 {
  top: 4825px;
  left: 4650px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart - Jugular Venous Distention */
  /* Transform skew can help with rotation and tilting of the line */
  img.image17 {
  top: 4550px;
  left: 4450px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Lower Limb Low Blood Pressure Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image18 {
  top: 4115px;
  left: 3810px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Lower Limb Low Blood Pressure Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image19 {
  top: 3950px;
  left: 3850px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart - Lower Limb Low Blood Pressure */
  /* Transform skew can help with rotation and tilting of the line */
  img.image20 {
  top: 4100px;
  left: 4000px;
  position: absolute;
  z-index: -5;
  }

    /* styles for Murmur Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image21 {
  top: 5130px;
  left: 4255px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Murmur Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image22 {
  top: 4965px;
  left: 4310px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart - Murmur */
  /* Transform skew can help with rotation and tilting of the line */
  img.image23 {
  top: 4535px;
  left: 4375px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Peripheral Edema Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image24 {
  top: 4780px;
  left: 4815px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Peripheral Edema Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image25 {
  top: 4625px;
  left: 4850px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart - Peripheral Edema */
  /* Transform skew can help with rotation and tilting of the line */
  img.image26 {
  top: 4475px;
  left: 4475px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Syncope Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image27 {
  top: 4800px;
  left: 3640px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Syncope Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image28 {
  top: 4625px;
  left: 3700px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart - Syncope */
  /* Transform skew can help with rotation and tilting of the line */
  img.image29 {
  top: 4475px;
  left: 3930px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Weight Loss Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image30 {
  top: 4525px;
  left: 4960px;
  position: absolute;
  z-index: -.5;
  }

    /* styles for Wight Loss Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image31 {
  top: 4365px;
  left: 5010px;
  position: absolute;
  z-index: -3;
  }

    /* styles for Heart - Weight Loss */
  /* Transform skew can help with rotation and tilting of the line */
  img.image32 {
  top: 4435px;
  left: 4475px;
  position: absolute;
  z-index: -4;
  }

    /* styles for Substernal Chest Pain Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image33 {
  top: 3325px;
  left: 4250px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Substernal Chest Pain Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image34 {
  top: 3165px;
  left: 4310px;
  position: absolute;
  z-index: -4;
  }  

    /* styles for Cyanosis Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image39 {
  top: 4525px;
  left: 2860px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Cyanosis Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image40 {
  top: 4365px;
  left: 2910px;
  position: absolute;
  z-index: -4;
  }   

    /* styles for Tearing Chest Pain Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image42 {
  top: 3425px;
  left: 3800px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Tearing Chest Pain Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image43 {
  top: 3265px;
  left: 3850px;
  position: absolute;
  z-index: -4;
  }         

    /* styles for Sharp Chest Pain Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image45 {
  top: 3425px;
  left: 4700px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Sharp Chest Pain Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image46 {
  top: 3265px;
  left: 4750px;
  position: absolute;
  z-index: -4;
  }  
  
    /* styles for Low Pitch Holosystolic Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image48 {
  top: 5660px;
  left: 4600px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Low Pitch Holosystolic Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image49 {
  top: 5500px;
  left: 4700px;
  position: absolute;
  z-index: -4;
  }        

    /* styles for CREAM Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image51 {
  top: 5225px;
  left: 5200px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for CREAM Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image52 {
  top: 5065px;
  left: 5250px;
  position: absolute;
  z-index: -4;
  }   

    /* styles for Red LL Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image54 {
  top: 4930px;
  left: 5400px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Red LL Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image55 {
  top: 4765px;
  left: 5450px;
  position: absolute;
  z-index: -4;
  }     
  
    /* styles for Decreased Heart Sound Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image57 {
  top: 5460px;
  left: 4925px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Decreased Heart Sound Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image58 {
  top: 5300px;
  left: 5000px;
  position: absolute;
  z-index: -4;
  }   
  
   /* styles for Tachycardia Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image60 {
  top: 5665px;
  left: 3855px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Tachycardia Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image61 {
  top: 5500px;
  left: 3900px;
  position: absolute;
  z-index: -4;
  }  
  
   /* styles for Bradycardia Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image63 {
  top: 5460px;
  left: 3510px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Bradycardia Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image64 {
  top: 5300px;
  left: 3550px;
  position: absolute;
  z-index: -4;
  }  

   /* styles for Back Pain Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image66 {
  top: 5235px;
  left: 3225px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Back Pain Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image67 {
  top: 5065px;
  left: 3250px;
  position: absolute;
  z-index: -4;
  }  

   /* styles for Baseline Asymptomatic Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image69 {
  top: 4925px;
  left: 2960px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Baseline Asymptomatic Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image70 {
  top: 4765px;
  left: 3050px;
  position: absolute;
  z-index: -4;
  }  
  
   /* styles for Hypotension Phrase */
  /* Transform skew can help with rotation and tilting of the line */
  img.image72 {
  top: 5900px;
  left: 5325px;
  position: absolute;
  z-index: -.5;
  }  

    /* styles for Hypotension Button */
  /* Transform skew can help with rotation and tilting of the line */
  img.image73 {
  top: 5735px;
  left: 5435px;
  position: absolute;
  z-index: -4;
  }  

  /* styles for Uremic Pericarditis Card */
  img.image75 {
  top: 2155px;
  left: 5090px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Uremic Pericarditis Button */
  img.image76 {
  top: 2805px;
  left: 5090px;
  position: absolute;
  z-index: -1;
  }    

  /* styles for Chagas Disease Card */
  img.image77 {
  top: 3550px;
  left: 5000px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Chagas Disease Button */
  img.image78 {
  top: 3550px;
  left: 5000px;
  position: absolute;
  z-index: -1;
  }    

  /* styles for Infective Endocarditis Card */
  img.image79 {
  top: 3950px;
  left: 5200px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Infective Endocarditis Button */
  img.image80 {
  top: 3950px;
  left: 5200px;
  position: absolute;
  z-index: -1;
  }      

  /* styles for Atrial Myxoma Card */
  img.image81 {
  top: 4365px;
  left: 5510px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Atrial Myxoma Button */
  img.image82 {
  top: 4365px;
  left: 5510px;
  position: absolute;
  z-index: -1;
  }        

  /* styles for Deep Venous Thrombosis Card */
  img.image83 {
  top: 4965px;
  left: 5910px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Deep Venous Thrombosis Button */
  img.image84 {
  top: 4965px;
  left: 5910px;
  position: absolute;
  z-index: -1;
  }    

  /* styles for Kawasakis Disease Card */
  img.image85 {
  top: 5400px;
  left: 5650px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Kawasakis Disease Button */
  img.image86 {
  top: 5400px;
  left: 5650px;
  position: absolute;
  z-index: -1;
  }      

  /* styles for Cardiac Tamponade Card */
  img.image87 {
  top: 6100px;
  left: 6050px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Cardiac Tamponade Button */
  img.image88 {
  top: 6100px;
  left: 6050px;
  position: absolute;
  z-index: -1;
  }        

  /* styles for Pericardial Effusion Card */
  img.image89 {
    top: 6400px;
  left: 5550px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Pericardial Effusion Button */
  img.image90 {
  top: 6400px;
  left: 5550px;
  position: absolute;
  z-index: -1;
  }       

  /* styles for Mitral Regurgitation Card */
  img.image91 {
  top: 6000px;
  left: 4850px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Mitral Regurgitation Button */
  img.image92 {
  top: 6000px;
  left: 4850px;
  position: absolute;
  z-index: -1;
  }       
  
  /* styles for Atrial Flutter Card */
  img.image93 {
    top: 6000px;
  left: 3950px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Atrial Flutter Button */
  img.image94 {
  top: 6000px;
  left: 3950px;
  position: absolute;
  z-index: -1;
  }  
  
  /* styles for Atrial Fibrillation Card */
  img.image95 {
  top: 6000px;
  left: 3450px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Atrial Fibrillation Button */
  img.image96 {
  top: 6000px;
  left: 3450px;
  position: absolute;
  z-index: -1;
  }    

  /* styles for 2 AV Block Card */
  img.image97 {
  top: 5800px;
  left: 3050px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for 2 AV Block Button */
  img.image98 {
  top: 5800px;
  left: 3050px;
  position: absolute;
  z-index: -1;
  }      

  /* styles for Abdominal Aortic Aneurysm Card */
  img.image99 {
  top: 5500px;
  left: 2650px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Abdominal Aortic Aneurysm Button */
  img.image100 {
  top: 5500px;
  left: 2650px;
  position: absolute;
  z-index: -1;
  }     

  /* styles for Premature Ventricular Contraction Card */
  img.image101 {
  top: 5100px;
  left: 2250px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Premature Ventricular Contraction Button */
  img.image102 {
  top: 5100px;
  left: 2250px;
  position: absolute;
  z-index: -1;
  }       

  /* styles for Transposition of the Great Vessels Card */
  img.image103 {
  top: 4600px;
  left: 1950px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Transposition of the Great Vessels Button */
  img.image104 {
  top: 4600px;
  left: 1950px;
  position: absolute;
  z-index: -1;
  }       

  /* styles for Tetrallogy of Fallot Card */
  img.image105 {
  top: 4200px;
  left: 1980px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Tetrallogy of Fallot Button */
  img.image106 {
  top: 4200px;
  left: 1980px;
  position: absolute;
  z-index: -1;
  }     

  /* styles for Coarctation of the Aorta Card */
  img.image107 {
  top: 3700px;
  left: 2880px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Coarctation of the Aorta Button */
  img.image108 {
  top: 3700px;
  left: 2880px;
  position: absolute;
  z-index: -1;
  }      

  /* styles for Aortic Dissection Card */
  img.image109 {
  top: 3300px;
  left: 3180px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Aortic Dissection Button */
  img.image110 {
  top: 3300px;
  left: 3180px;
  position: absolute;
  z-index: -1;
  }      
  
    /* styles for Hypertrophic Obstructive Cardiomyopathy Card */
  img.image111 {
  top: 5565px;
  left: 4240px;
  position: absolute;
  z-index: -.3;
  }  

    /* styles for Hypertrophic Obstructive Cardiomyopathy Button */
  img.image112 {
  top: 5565px;
  left: 4240px;
  position: absolute;
  z-index: -4;
  }  

    /* styles for Improve with Rest Phrase */
  img.image113 {
  top: 2675px;
  left: 4280px;
  position: absolute;
  z-index: -.5;
  }    

    /* styles for Improve with Rest Button */
  img.image114 {
  top: 2503px;
  left: 4300px;
  position: absolute;
  z-index: -4;
  }    
  
    /* styles for Improve with Rest Line */
  img.image115 {
  top: 2903px;
  left: 4347px;
  position: absolute;
  z-index: -4;
  }      

  /* styles for Emotional Distress Phrase */
  img.image116 {
  top: 2675px;
  left: 4980px;
  position: absolute;
  z-index: -4;
  }    

  /* styles for Emotional Distress Button */
  img.image117 {
  top: 2503px;
  left: 5000px;
  position: absolute;
  z-index: -4;
  }    
  
  /* styles for Emotional Distress Line */
  img.image118 {
  top: 2903px;
  left: 4347px;
  position: absolute;
  z-index: -4;
  }        

  /* styles for Stable Angina Card */
  img.image119 {
  top: 2503px;
  left: 3600px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Stable Angina Button */
  img.image120 {
  top: 2503px;
  left: 3600px;
  position: absolute;
  z-index: -1;
  }    
  
  /* styles for Unstable Angina Card */
  img.image121 {
  top: 2150px;
  left: 3800px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Unstable Angina Button */
  img.image122 {
  top: 2150px;
  left: 3800px;
  position: absolute;
  z-index: -1;
  }    
  
  /* styles for None ST Elevated Myocardial Infarction Card */
  img.image123 {
  top: 1903px;
  left: 4220px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for None ST Elevated Myocardial Infarction Button */
  img.image124 {
  top: 1903px;
  left: 4220px;
  position: absolute;
  z-index: -1;
  }    
  
  /* styles for ST Elevated Myocardial Infarction Card */
  img.image125 {
  top: 2150px;
  left: 4700px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for ST Elevated Myocardial Infarction Button */
  img.image126 {
  top: 2150px;
  left: 4700px;
  position: absolute;
  z-index: -1;
  }    
  
  /* styles for Takatsubos Disease Card */
  img.image127 {
  top: 2503px;
  left: 5500px;
  position: absolute;
  z-index: -.3;
  }

  /* styles for Takatsubos Disease Button */
  img.image128 {
  top: 2503px;
  left: 5500px;
  position: absolute;
  z-index: -1;
  }      

  /* styles for Murmur - Hypertrophic Obstructive Cardiomyopathy */
  img.image129 {
  top: 5140px;
  left: 4375px;
  position: absolute;
  z-index: -1;
  }        

  /* styles for Palpitations - Hypertrophic Obstructive Cardiomyopathy */
  img.image130 {
  top: 4970px;
  left: 4050px;
  position: absolute;
  z-index: -1;
  }          

  /* styles for Murmur - Low Pitch Holosystolic */
  img.image131 {
  top: 5125px;
  left: 4475px;
  position: absolute;
  z-index: -1;
  }   
  
  /* styles for Low Pitch Holosystolic - Mitral Regurgitation */
  img.image132 {
  top: 5670px;
  left: 4850px;
  position: absolute;
  z-index: -1;
  }     

  /* styles for Palpitation - Tachycardia */
  img.image133 {
  top: 5015px;
  left: 3975px;
  position: absolute;
  z-index: -1;
  }    

  /* styles for Tachycardia - Atrial Flutter */
  img.image134 {
  top: 5675px;
  left: 3985px;
  position: absolute;
  z-index: -1;
  }      

  /* styles for Tachycardia - Atrial Fibrillation */
  img.image135 {
  top: 5625px;
  left: 3625px;
  position: absolute;
  z-index: -1;
  }     

  /* styles for Palpitation - Bradycardia */
  img.image136 {
  top: 5000px;
  left: 3700px;
  position: absolute;
  z-index: -1;
  }     

  /* styles for Bradycardia - 2 AV Block */
  img.image137 {
  top: 5450px;
  left: 3225px;
  position: absolute;
  z-index: -1;
  }       

  /* styles for Syncope - Back Pain */
  img.image138 {
  top: 4775px;
  left: 3400px;
  position: absolute;
  z-index: -1;
  }     
  
  /* styles for Back Pain - Abdominal Aortic Aneurysm */
  img.image139 {
  top: 5175px;
  left: 2900px;
  position: absolute;
  z-index: -1;
  }    
  
  /* styles for Syncope - Asymptomatic Baseline */
  img.image140 {
  top: 4700px;
  left: 3250px;
  position: absolute;
  z-index: -1;
  }       

  /* styles for Asymptomatic Baseline - Premature Ventricular Contraction */
  img.image141 {
  top: 4875px;
  left: 2575px;
  position: absolute;
  z-index: -1;
  }      

  /* styles for Neonate - Blue Cyanosis */
  img.image142 {
  top: 4425px;
  left: 3090px;
  position: absolute;
  z-index: -3;
  }  
  /* styles for Blue Cyanosis - Transposition of the Great Vessels */
  img.image143 {
  top: 4475px;
  left: 2450px;
  position: absolute;
  z-index: -3;
  }    

  /* styles for Blue Cyanosis - Tetrallogy of Fallot */
  img.image144 {
  top: 4250px;
  left: 2420px;
  position: absolute;
  z-index: -3;
  }     

  /* styles for Lower Limb - Coarctation of the Aorta */
  img.image145 {
  top: 3775px;
  left: 3320px;
  position: absolute;
  z-index: -3;
  }      

  /* styles for Lower Limb - Aortic Dissection */
  img.image146 {
  top: 3475px;
  left: 3520px;
  position: absolute;
  z-index: -3;
  }     

  /* styles for Chest Pain - Tearing Chest Pain */
  img.image147 {
  top: 3400px;
  left: 4000px;
  position: absolute;
  z-index: -3;
  }       

  /* styles for Tearing Chest Pain - Aortic Dissection */
  img.image148 {
  top: 3340px;
  left: 3540px;
  position: absolute;
  z-index: -3;
  }      

  /* styles for  Chest Pain - Substernal Chest Pain */
  img.image149 {
  top: 3335px;
  left: 4375px;
  position: absolute;
  z-index: -3;
  }        

  /* styles for  Chest Pain - Sharp Chest Pain */
  img.image150 {
  top: 3410px;
  left: 4450px;
  position: absolute;
  z-index: -3;
  }      

  /* styles for  Fever - Chagas */
  img.image151 {
  top: 3710px;
  left: 4925px;
  position: absolute;
  z-index: -3;
  }     
  
  /* styles for  Fever - Infective Endocarditis */
  img.image152 {
  top: 4010px;
  left: 4975px;
  position: absolute;
  z-index: -3;
  }        

  /* styles for  Weight Loss - Atrial Myxoma */
  img.image153 {
  top: 4425px;
  left: 5185px;
  position: absolute;
  z-index: -3;
  }         
  
  /* styles for  Weight Loss - Infective Endocarditis */
  img.image154 {
  top: 4125px;
  left: 5095px;
  position: absolute;
  z-index: -3;
  }            

  /* styles for  Peripheral Edema - Red Lower Limb */
  img.image155 {
  top: 4725px;
  left: 5025px;
  position: absolute;
  z-index: -3;
  }        

  /* styles for  Red Lower Limb - Deep Venous Thrombosis */
  img.image156 {
  top: 4878px;
  left: 5600px;
  position: absolute;
  z-index: -3;
  }          

  /* styles for  Peripheral Edema - CREAM */
  img.image157 {
  top: 4925px;
  left: 4815px;
  position: absolute;
  z-index: -3;
  }     

  /* styles for  CREAM - Kawasakis Disease */
  img.image158 {
  top: 5200px;
  left: 5370px;
  position: absolute;
  z-index: -3;
  }   

  /* styles for  Peripheral Edema - Decreased Heart Sound */
  img.image159 {
  top: 4975px;
  left: 4750px;
  position: absolute;
  z-index: -3;
  }     

  /* styles for  Decreased Heart Sound - Hypotension */
  img.image160 {
  top: 5425px;
  left: 5150px;
  position: absolute;
  z-index: -3;
  }      

  /* styles for  Hypotension - Pulmonary Embolism */
  img.image161 {
  top: 5890px;
  left: 5540px;
  position: absolute;
  z-index: -3;
  }      
  
  /* styles for  Hypotension - Cardiac Tamponade */
  img.image162 {
  top: 5810px;
  left: 5600px;
  position: absolute;
  z-index: -3;
  }     
  
  /* styles for  Substernal Chest Pain - Improve with Rest */
  img.image163 {
  top: 2680px;
  left: 4375px;
  position: absolute;
  z-index: -3;
  }        
  
  /* styles for  Improve with Rest - None ST Elevated Myocardial Infarction */
  img.image164 {
  top: 2080px;
  left: 4375px;
  position: absolute;
  z-index: -3;
  }   
  
  /* styles for  Sharp Chest Pain - Uremic Pericarditis */
  img.image165 {
  top: 2980px;
  left: 4900px;
  position: absolute;
  z-index: -3;
  }   

  /* styles for  Singularity 1 - Emotional Distress */
  img.image166 {
  top: 2575px;
  left: 4475px;
  position: absolute;
  z-index: -3;
  }     

  /* styles for  Emotional Distress - Takatsubos Disease */
  img.image167 {
  top: 2575px;
  left: 5175px;
  position: absolute;
  z-index: -3;
  }       

  /* styles for  Singularity 1 - Stable Angina */
  img.image168 {
  top: 2575px;
  left: 3850px;
  position: absolute;
  z-index: -3;
  }     

  /* styles for  Singularity 1 - Unstable Angina */
  img.image169 {
  top: 2325px;
  left: 4100px;
  position: absolute;
  z-index: -3;
  }       

  /* styles for  Singularity 1 - ST Myocardial Infarction */
  img.image170 {
  top: 2325px;
  left: 4450px;
  position: absolute;
  z-index: -3;
  }      
</style>

