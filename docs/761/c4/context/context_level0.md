@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Container.puml
!define DEVICONS https://raw.githubusercontent.com/tupadr3/plantuml-icon-font-sprites/master/devicons
!define FONTAWESOME https://raw.githubusercontent.com/tupadr3/plantuml-icon-font-sprites/master/font-awesome-5
!include FONTAWESOME/mobile.puml
LAYOUT_WITH_LEGEND()
LAYOUT_LANDSCAPE()
AddRelTag("dashed", $lineStyle = DashedLine())
System(761_FxPub, "761_FxPub", "", "", "" , "")
System_Ext(257_EAI, "257_EAI", "", "", "" , "")
System_Ext(21_CASA, "21_CASA", "", "", "" , "")
System_Ext(30_AAA, "30_AAA", "", "", "" , "")
System_Ext(100_CCC, "100_CCC", "", "", "" , "")
System_Ext(1000_DDD, "1000_DDD", "", "", "" , "")
System_Ext(760_ForeignCASA, "760_ForeignCASA", "", "", "" , "")

Rel(761_FxPub, 257_EAI, "Online", "", "", "", "" , "")
Rel(761_FxPub, 30_AAA, "Online", "", "", "", "" , "")
Rel(761_FxPub, 100_CCC, "Online", "", "", "", "" , "")
Rel(761_FxPub, 1000_DDD, "Online", "", "", "", "" , "")
Rel(257_EAI, 21_CASA, "Online", "", "", "", "" , "")
Rel(257_EAI, 760_ForeignCASA, "Online", "", "", "", "" , "")
@enduml
