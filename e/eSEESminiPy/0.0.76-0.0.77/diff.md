# Comparing `tmp/eSEESminiPy-0.0.76-py3-none-any.whl.zip` & `tmp/eSEESminiPy-0.0.77-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 844990 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     5118 b- defN 23-Mar-13 01:47 eSEESminiPy/__init__ - Copy.py
--rw-rw-rw-  2.0 fat     5233 b- defN 23-Mar-13 02:11 eSEESminiPy/__init__.py
--rw-rw-rw-  2.0 fat  2250752 b- defN 23-Mar-13 21:49 eSEESminiPy/eSEESminiPy.pyd
--rw-rw-rw-  2.0 fat     4674 b- defN 23-Mar-13 21:50 eSEESminiPy-0.0.76.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-13 21:50 eSEESminiPy-0.0.76.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Mar-13 21:50 eSEESminiPy-0.0.76.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      572 b- defN 23-Mar-13 21:50 eSEESminiPy-0.0.76.dist-info/RECORD
-7 files, 2266453 bytes uncompressed, 843980 bytes compressed:  62.8%
+Zip file size: 851883 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     5204 b- defN 23-Jun-01 01:51 eSEESminiPy/__init__.py
+-rw-rw-rw-  2.0 fat  2266112 b- defN 23-Jun-01 01:46 eSEESminiPy/eSEESminiPy.pyd
+-rw-rw-rw-  2.0 fat     5764 b- defN 23-Jun-01 01:56 eSEESminiPy-0.0.77.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 01:56 eSEESminiPy-0.0.77.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-01 01:56 eSEESminiPy-0.0.77.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      485 b- defN 23-Jun-01 01:56 eSEESminiPy-0.0.77.dist-info/RECORD
+6 files, 2277669 bytes uncompressed, 851009 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
-Filename: eSEESminiPy/__init__ - Copy.py
-Comment: 
-
 Filename: eSEESminiPy/__init__.py
 Comment: 
 
 Filename: eSEESminiPy/eSEESminiPy.pyd
 Comment: 
 
-Filename: eSEESminiPy-0.0.76.dist-info/METADATA
+Filename: eSEESminiPy-0.0.77.dist-info/METADATA
 Comment: 
 
-Filename: eSEESminiPy-0.0.76.dist-info/WHEEL
+Filename: eSEESminiPy-0.0.77.dist-info/WHEEL
 Comment: 
 
-Filename: eSEESminiPy-0.0.76.dist-info/top_level.txt
+Filename: eSEESminiPy-0.0.77.dist-info/top_level.txt
 Comment: 
 
-Filename: eSEESminiPy-0.0.76.dist-info/RECORD
+Filename: eSEESminiPy-0.0.77.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## eSEESminiPy/__init__.py

```diff
@@ -1,115 +1,117 @@
-from .eSEESminiPy import ApplyDamping
-from .eSEESminiPy import buildFiberSection
-from .eSEESminiPy import buildGeneralizedFiberSection
-from .eSEESminiPy import buildModelData
-from .eSEESminiPy import BuildRCrectSection
-from .eSEESminiPy import buildSection
-from .eSEESminiPy import buildStandardWsectionFiber
-from .eSEESminiPy import buildWsectionFiber
-from .eSEESminiPy import clearPlotExtras
-from .eSEESminiPy import createFigBucket
-from .eSEESminiPy import defineStrainHistory
-from .eSEESminiPy import DisplayModelDataTables
-from .eSEESminiPy import displayOSmodel
-from .eSEESminiPy import displayOSmodelWithHinges
-from .eSEESminiPy import DisplayOutputTables
-from .eSEESminiPy import drawAFD
-from .eSEESminiPy import drawBMD
-from .eSEESminiPy import drawCircLayer
-from .eSEESminiPy import drawCircularPatch
-from .eSEESminiPy import DrawCurvatures
-from .eSEESminiPy import drawCurvatures
-from .eSEESminiPy import DrawDeformedShape
-from .eSEESminiPy import drawDeformedShape
-from .eSEESminiPy import drawDeformedShape3D
-from .eSEESminiPy import DrawElementResponse
-from .eSEESminiPy import drawFiberSection
-from .eSEESminiPy import DrawModel
-from .eSEESminiPy import drawModel
-from .eSEESminiPy import DrawModeShape
-from .eSEESminiPy import DrawModeShapes
-from .eSEESminiPy import DrawMUy
-from .eSEESminiPy import drawOneFiber
-from .eSEESminiPy import DrawPlasticRotations
-from .eSEESminiPy import drawPlasticRotations
-from .eSEESminiPy import drawQuadPatch
-from .eSEESminiPy import drawQuadrilateralPatch
-from .eSEESminiPy import drawQuick2DModelFrame
-from .eSEESminiPy import drawQuick3DModelFrame
-from .eSEESminiPy import drawRectPatch
-from .eSEESminiPy import DrawRotations
-from .eSEESminiPy import drawRotations
-from .eSEESminiPy import drawSFD
-from .eSEESminiPy import DrawStoryDrift
-from .eSEESminiPy import drawStraightLayer
-from .eSEESminiPy import DrawThis
-from .eSEESminiPy import evalFx
-from .eSEESminiPy import formatAx
-from .eSEESminiPy import formatAx3D
-from .eSEESminiPy import getAllElementForces
-from .eSEESminiPy import getAllElementForcesMax
-from .eSEESminiPy import getAllElementResponse_AllSectionDefo
-from .eSEESminiPy import getAllNodeDisp
-from .eSEESminiPy import getAnalysisParametersDynamic
-from .eSEESminiPy import getAnalysisParametersStatic
-from .eSEESminiPy import getAnalysisResults
-from .eSEESminiPy import getColorList
-from .eSEESminiPy import getColorListBlueGrays
-from .eSEESminiPy import getColorListGrays
-from .eSEESminiPy import getCommandDataRectPatchCoreWithCover
-from .eSEESminiPy import getElementForces
-from .eSEESminiPy import getFiberCommands_Wsection
-from .eSEESminiPy import getFiberSectionCommandData
-from .eSEESminiPy import getHSSsectionData
-from .eSEESminiPy import getInputArray_AggregatorSection
-from .eSEESminiPy import getIntegrationGaussLobattoQuadratureLocs
-from .eSEESminiPy import getIntegrationGaussLobattoQuadratureWts
-from .eSEESminiPy import getIntegrationWeights_LowOrderBeamIntegration
-from .eSEESminiPy import getKWargsDefaultsModelView
-from .eSEESminiPy import getMaterialInputArray
-from .eSEESminiPy import getMaterialStressStrain
-from .eSEESminiPy import getModelElementData
-from .eSEESminiPy import getModelNodeData
-from .eSEESminiPy import getPeriods
-from .eSEESminiPy import GetPeriods
-from .eSEESminiPy import getSectionLocationsHingeRadauBeamIntegration
-from .eSEESminiPy import getSectionLocationsHingeRadauTwoBeamIntegration
-from .eSEESminiPy import getWeightsHingeRadauBeamIntegration
-from .eSEESminiPy import getWeightsHingeRadauTwoBeamIntegration
-from .eSEESminiPy import getWsectionData
-from .eSEESminiPy import InitializeAll
-from .eSEESminiPy import initializeOutputSwitches
-from .eSEESminiPy import makeCommandButton
-from .eSEESminiPy import makeCommandButtonWithLabel
-from .eSEESminiPy import makeFigAx
-from .eSEESminiPy import makeFigAxSized
-from .eSEESminiPy import ops_recorder
-from .eSEESminiPy import plotFx
-from .eSEESminiPy import plotXY
-from .eSEESminiPy import plotXYoneList
-from .eSEESminiPy import plotYoneList
-from .eSEESminiPy import printMomentCurvatureExample
-from .eSEESminiPy import ReadSMDFileToList
-from .eSEESminiPy import removeAxisLabels
-from .eSEESminiPy import removePlotBorder
-from .eSEESminiPy import reverseDictionaryLookup
-from .eSEESminiPy import reverseXaxis
-from .eSEESminiPy import reverseYaxis
-from .eSEESminiPy import rotateVector3D
-from .eSEESminiPy import round_to_N
-from .eSEESminiPy import RunCyclicStaticAnalysis
-from .eSEESminiPy import RunEQDynamicAnalysis
-from .eSEESminiPy import runMomentCurvature
-from .eSEESminiPy import runOpenSees_SDOF_Transient
-from .eSEESminiPy import runOpenSeesSDOF_elastic
-from .eSEESminiPy import runQuickGravityAnalysis
-from .eSEESminiPy import runQuickStaticAnalysis
-from .eSEESminiPy import RunStaticElasticFrameAnalysisInOpenSeesPy
-from .eSEESminiPy import SavePlotFigures
-from .eSEESminiPy import set_aspect_equal_3d
-from .eSEESminiPy import setDarkBackground
-from .eSEESminiPy import setKWarg
-from .eSEESminiPy import setMyUnits
-from .eSEESminiPy import testMaterial
-from .eSEESminiPy import transformAxes3D
-from .eSEESminiPy import transformAxes3DTitles
+from eSEESminiPy import ApplyDamping
+from eSEESminiPy import buildFiberSection
+from eSEESminiPy import buildGeneralizedFiberSection
+from eSEESminiPy import buildModelData
+from eSEESminiPy import BuildRCrectSection
+from eSEESminiPy import buildSection
+from eSEESminiPy import buildStandardWsectionFiber
+from eSEESminiPy import buildWsectionFiber
+from eSEESminiPy import clearPlotExtras
+from eSEESminiPy import createFigBucket
+from eSEESminiPy import defineStrainHistory
+from eSEESminiPy import DisplayModelDataTables
+from eSEESminiPy import displayOSmodel
+from eSEESminiPy import displayOSmodelWithHinges
+from eSEESminiPy import DisplayOutputTables
+from eSEESminiPy import drawAFD
+from eSEESminiPy import drawBMD
+from eSEESminiPy import drawCircLayer
+from eSEESminiPy import drawCircularPatch
+from eSEESminiPy import DrawCurvatures
+from eSEESminiPy import drawCurvatures
+from eSEESminiPy import DrawDeformedShape
+from eSEESminiPy import drawDeformedShape
+from eSEESminiPy import drawDeformedShape3D
+from eSEESminiPy import DrawElementResponse
+from eSEESminiPy import drawFiberSection
+from eSEESminiPy import DrawModel
+from eSEESminiPy import drawModel
+from eSEESminiPy import DrawModeShape
+from eSEESminiPy import DrawModeShapes
+from eSEESminiPy import DrawMUy
+from eSEESminiPy import drawOneFiber
+from eSEESminiPy import DrawPlasticRotations
+from eSEESminiPy import drawPlasticRotations
+from eSEESminiPy import drawQuadPatch
+from eSEESminiPy import drawQuadrilateralPatch
+from eSEESminiPy import drawQuick2DModelFrame
+from eSEESminiPy import drawQuick3DModelFrame
+from eSEESminiPy import drawRectPatch
+from eSEESminiPy import DrawRotations
+from eSEESminiPy import drawRotations
+from eSEESminiPy import drawSFD
+from eSEESminiPy import DrawStoryDrift
+from eSEESminiPy import drawStraightLayer
+from eSEESminiPy import DrawThis
+from eSEESminiPy import evalFx
+from eSEESminiPy import formatAx
+from eSEESminiPy import formatAx3D
+from eSEESminiPy import getAllElementForces
+from eSEESminiPy import getAllElementForcesMax
+from eSEESminiPy import getAllElementResponse_AllSectionDefo
+from eSEESminiPy import getAllNodeDisp
+from eSEESminiPy import getAnalysisParametersDynamic
+from eSEESminiPy import getAnalysisParametersStatic
+from eSEESminiPy import getAnalysisResults
+from eSEESminiPy import getColorList
+from eSEESminiPy import getColorListBlueGrays
+from eSEESminiPy import getColorListGrays
+from eSEESminiPy import getCommandDataRectPatchCoreWithCover 
+from eSEESminiPy import getElementForces
+from eSEESminiPy import getFiberCommands_Wsection
+from eSEESminiPy import getFiberSectionCommandData
+from eSEESminiPy import getHSSsectionData
+from eSEESminiPy import getInputArray_AggregatorSection
+from eSEESminiPy import getIntegrationGaussLobattoQuadratureLocs
+from eSEESminiPy import getIntegrationGaussLobattoQuadratureWts
+from eSEESminiPy import getIntegrationWeights_LowOrderBeamIntegration
+from eSEESminiPy import getKWargsDefaultsModelView
+from eSEESminiPy import getLocalsDict
+from eSEESminiPy import getLocalsDictNumbers
+from eSEESminiPy import getMaterialInputArray
+from eSEESminiPy import getMaterialStressStrain
+from eSEESminiPy import getModelElementData
+from eSEESminiPy import getModelNodeData
+from eSEESminiPy import getPeriods
+from eSEESminiPy import GetPeriods
+from eSEESminiPy import getSectionLocationsHingeRadauBeamIntegration
+from eSEESminiPy import getSectionLocationsHingeRadauTwoBeamIntegration
+from eSEESminiPy import getWeightsHingeRadauBeamIntegration
+from eSEESminiPy import getWeightsHingeRadauTwoBeamIntegration
+from eSEESminiPy import getWsectionData
+from eSEESminiPy import InitializeAll
+from eSEESminiPy import initializeOutputSwitches
+from eSEESminiPy import makeCommandButton
+from eSEESminiPy import makeCommandButtonWithLabel
+from eSEESminiPy import makeFigAx
+from eSEESminiPy import makeFigAxSized
+from eSEESminiPy import ops_recorder
+from eSEESminiPy import plotFx
+from eSEESminiPy import plotXY
+from eSEESminiPy import plotXYoneList
+from eSEESminiPy import plotYoneList
+from eSEESminiPy import printMomentCurvatureExample
+from eSEESminiPy import ReadSMDFileToList
+from eSEESminiPy import removeAxisLabels
+from eSEESminiPy import removePlotBorder
+from eSEESminiPy import reverseDictionaryLookup
+from eSEESminiPy import reverseXaxis
+from eSEESminiPy import reverseYaxis
+from eSEESminiPy import rotateVector3D
+from eSEESminiPy import round_to_N
+from eSEESminiPy import RunCyclicStaticAnalysis
+from eSEESminiPy import RunEQDynamicAnalysis
+from eSEESminiPy import runMomentCurvature
+from eSEESminiPy import runOpenSees_SDOF_Transient
+from eSEESminiPy import runOpenSeesSDOF_elastic
+from eSEESminiPy import runQuickGravityAnalysis
+from eSEESminiPy import runQuickStaticAnalysis
+from eSEESminiPy import RunStaticElasticFrameAnalysisInOpenSeesPy
+from eSEESminiPy import SavePlotFigures
+from eSEESminiPy import set_aspect_equal_3d
+from eSEESminiPy import setDarkBackground
+from eSEESminiPy import setKWarg
+from eSEESminiPy import setMyUnits
+from eSEESminiPy import testMaterial
+from eSEESminiPy import transformAxes3D
+from eSEESminiPy import transformAxes3DTitles
```

## Comparing `eSEESminiPy-0.0.76.dist-info/METADATA` & `eSEESminiPy-0.0.77.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eSEESminiPy
-Version: 0.0.76
+Version: 0.0.77
 Summary: A Series of function to create an OpenSees Model
 Author: Silvia Mazzoni
 Author-email: <silviamazzoni@yahoo.com>
 License: UNKNOWN
 Keywords: python,Openseespy
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -17,102 +17,126 @@
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: openseespy
 
 ## This package was developed by Silvia Mazzoni, silviamazzoni@yahoo.com
 
 ## USAGE
-from eSEESminiPy import round_to_N
-from eSEESminiPy import setMyUnits
-from eSEESminiPy import plotYoneList
-from eSEESminiPy import plotXYoneList
-from eSEESminiPy import plotXY
-from eSEESminiPy import DrawModeShape
-from eSEESminiPy import DrawModeShapes
-from eSEESminiPy import drawModel
-from eSEESminiPy import DrawModel
-from eSEESminiPy import set_aspect_equal_3d
-from eSEESminiPy import drawQuick3DModelFrame
-from eSEESminiPy import drawQuick2DModelFrame
-from eSEESminiPy import drawDeformedShape3D
-from eSEESminiPy import setKWarg
-from eSEESminiPy import getKWargsDefaultsModelView
+from eSEESminiPy import ApplyDamping
+from eSEESminiPy import buildFiberSection
+from eSEESminiPy import buildGeneralizedFiberSection
+from eSEESminiPy import buildModelData
+from eSEESminiPy import BuildRCrectSection
+from eSEESminiPy import buildSection
+from eSEESminiPy import buildStandardWsectionFiber
+from eSEESminiPy import buildWsectionFiber
+from eSEESminiPy import clearPlotExtras
 from eSEESminiPy import createFigBucket
+from eSEESminiPy import defineStrainHistory
+from eSEESminiPy import DisplayModelDataTables
+from eSEESminiPy import displayOSmodel
+from eSEESminiPy import displayOSmodelWithHinges
+from eSEESminiPy import DisplayOutputTables
+from eSEESminiPy import drawAFD
+from eSEESminiPy import drawBMD
+from eSEESminiPy import drawCircLayer
+from eSEESminiPy import drawCircularPatch
+from eSEESminiPy import DrawCurvatures
+from eSEESminiPy import drawCurvatures
 from eSEESminiPy import DrawDeformedShape
 from eSEESminiPy import drawDeformedShape
-from eSEESminiPy import getElementForces
+from eSEESminiPy import drawDeformedShape3D
+from eSEESminiPy import DrawElementResponse
+from eSEESminiPy import drawFiberSection
+from eSEESminiPy import DrawModel
+from eSEESminiPy import drawModel
+from eSEESminiPy import DrawModeShape
+from eSEESminiPy import DrawModeShapes
 from eSEESminiPy import DrawMUy
-from eSEESminiPy import DrawRotations
+from eSEESminiPy import drawOneFiber
 from eSEESminiPy import DrawPlasticRotations
-from eSEESminiPy import DrawCurvatures
-from eSEESminiPy import drawRotations
 from eSEESminiPy import drawPlasticRotations
-from eSEESminiPy import drawCurvatures
-from eSEESminiPy import DrawElementResponse
-from eSEESminiPy import clearPlotExtras
-from eSEESminiPy import setDarkBackground
-from eSEESminiPy import removePlotBorder
-from eSEESminiPy import drawBMD
-from eSEESminiPy import drawAFD
+from eSEESminiPy import drawQuadPatch
+from eSEESminiPy import drawQuadrilateralPatch
+from eSEESminiPy import drawQuick2DModelFrame
+from eSEESminiPy import drawQuick3DModelFrame
+from eSEESminiPy import drawRectPatch
+from eSEESminiPy import DrawRotations
+from eSEESminiPy import drawRotations
 from eSEESminiPy import drawSFD
 from eSEESminiPy import DrawStoryDrift
-from eSEESminiPy import displayOSmodel
-from eSEESminiPy import displayOSmodelWithHinges
-from eSEESminiPy import initializeOutputSwitches
-from eSEESminiPy import buildModelData
-from eSEESminiPy import RunStaticElasticFrameAnalysisInOpenSeesPy
-from eSEESminiPy import getAnalysisResults
-from eSEESminiPy import SavePlotFigures
-from eSEESminiPy import InitializeAll
+from eSEESminiPy import drawStraightLayer
 from eSEESminiPy import DrawThis
-from eSEESminiPy import DisplayModelDataTables
-from eSEESminiPy import DisplayOutputTables
-from eSEESminiPy import getWsectionData
-from eSEESminiPy import getHSSsectionData
-from eSEESminiPy import runMomentCurvature
-from eSEESminiPy import buildFiberSection
-from eSEESminiPy import getCommandDataRectPatchCoreWithCover
-from eSEESminiPy import getFiberSectionCommandData
-from eSEESminiPy import buildSection
-from eSEESminiPy import printMomentCurvatureExample
-from eSEESminiPy import plotFx
 from eSEESminiPy import evalFx
-from eSEESminiPy import getMaterialInputArray
-from eSEESminiPy import removeAxisLabels
 from eSEESminiPy import formatAx
 from eSEESminiPy import formatAx3D
-from eSEESminiPy import makeFigAx
-from eSEESminiPy import makeFigAxSized
-from eSEESminiPy import getInputArray_AggregatorSection
+from eSEESminiPy import getAllElementForces
+from eSEESminiPy import getAllElementForcesMax
+from eSEESminiPy import getAllElementResponse_AllSectionDefo
+from eSEESminiPy import getAllNodeDisp
+from eSEESminiPy import getAnalysisParametersDynamic
+from eSEESminiPy import getAnalysisParametersStatic
+from eSEESminiPy import getAnalysisResults
 from eSEESminiPy import getColorList
-from eSEESminiPy import getColorListGrays
 from eSEESminiPy import getColorListBlueGrays
-from eSEESminiPy import reverseXaxis
-from eSEESminiPy import reverseYaxis
-from eSEESminiPy import rotateVector3D
-from eSEESminiPy import transformAxes3D
-from eSEESminiPy import transformAxes3DTitles
-from eSEESminiPy import getIntegrationWeights_LowOrderBeamIntegration
-from eSEESminiPy import getIntegrationGaussLobattoQuadratureWts
+from eSEESminiPy import getColorListGrays
+from eSEESminiPy import getCommandDataRectPatchCoreWithCover 
+from eSEESminiPy import getElementForces
+from eSEESminiPy import getFiberCommands_Wsection
+from eSEESminiPy import getFiberSectionCommandData
+from eSEESminiPy import getHSSsectionData
+from eSEESminiPy import getInputArray_AggregatorSection
 from eSEESminiPy import getIntegrationGaussLobattoQuadratureLocs
+from eSEESminiPy import getIntegrationGaussLobattoQuadratureWts
+from eSEESminiPy import getIntegrationWeights_LowOrderBeamIntegration
+from eSEESminiPy import getKWargsDefaultsModelView
+from eSEESminiPy import getLocalsDict
+from eSEESminiPy import getLocalsDictNumbers
+from eSEESminiPy import getMaterialInputArray
+from eSEESminiPy import getMaterialStressStrain
+from eSEESminiPy import getModelElementData
+from eSEESminiPy import getModelNodeData
+from eSEESminiPy import getPeriods
+from eSEESminiPy import GetPeriods
 from eSEESminiPy import getSectionLocationsHingeRadauBeamIntegration
-from eSEESminiPy import getWeightsHingeRadauBeamIntegration
 from eSEESminiPy import getSectionLocationsHingeRadauTwoBeamIntegration
-from eSEESminiPy import getAllNodeDisp
-from eSEESminiPy import getAllElementForces
-from eSEESminiPy import getAllElementForcesMax
+from eSEESminiPy import getWeightsHingeRadauBeamIntegration
 from eSEESminiPy import getWeightsHingeRadauTwoBeamIntegration
-from eSEESminiPy import getPeriods
-from eSEESminiPy import GetPeriods
+from eSEESminiPy import getWsectionData
+from eSEESminiPy import InitializeAll
+from eSEESminiPy import initializeOutputSwitches
 from eSEESminiPy import makeCommandButton
 from eSEESminiPy import makeCommandButtonWithLabel
-from eSEESminiPy import reverseDictionaryLookup
-from eSEESminiPy import getAllElementResponse_AllSectionDefo
-from eSEESminiPy import BuildRCrectSection
+from eSEESminiPy import makeFigAx
+from eSEESminiPy import makeFigAxSized
+from eSEESminiPy import ops_recorder
+from eSEESminiPy import plotFx
+from eSEESminiPy import plotXY
+from eSEESminiPy import plotXYoneList
+from eSEESminiPy import plotYoneList
+from eSEESminiPy import printMomentCurvatureExample
 from eSEESminiPy import ReadSMDFileToList
+from eSEESminiPy import removeAxisLabels
+from eSEESminiPy import removePlotBorder
+from eSEESminiPy import reverseDictionaryLookup
+from eSEESminiPy import reverseXaxis
+from eSEESminiPy import reverseYaxis
+from eSEESminiPy import rotateVector3D
+from eSEESminiPy import round_to_N
+from eSEESminiPy import RunCyclicStaticAnalysis
+from eSEESminiPy import RunEQDynamicAnalysis
+from eSEESminiPy import runMomentCurvature
 from eSEESminiPy import runOpenSees_SDOF_Transient
-from eSEESminiPy import ApplyDamping
-from eSEESminiPy import getAnalysisParametersStatic
-from eSEESminiPy import getAnalysisParametersDynamic
-
+from eSEESminiPy import runOpenSeesSDOF_elastic
+from eSEESminiPy import runQuickGravityAnalysis
+from eSEESminiPy import runQuickStaticAnalysis
+from eSEESminiPy import RunStaticElasticFrameAnalysisInOpenSeesPy
+from eSEESminiPy import SavePlotFigures
+from eSEESminiPy import set_aspect_equal_3d
+from eSEESminiPy import setDarkBackground
+from eSEESminiPy import setKWarg
+from eSEESminiPy import setMyUnits
+from eSEESminiPy import testMaterial
+from eSEESminiPy import transformAxes3D
+from eSEESminiPy import transformAxes3DTitles
```

