# [hipermos-enhanced-freecad]  

- **Main Modifications:**
  -FreeCADBase
  1.[Console]Support output console infomation to log file.
  2.[Observer] Support focus Observer, while do some specific works.
  3.[Paraeter] fix some bugs and support check parameter is exist.
  4.[Placement]Rotation,Vector3D, fix bug of check equal caused by tolerance.
  5.[Sequencer] fix bug of show progress bar widget.
  6.[Tools] fix bug of get unique name.
  7.[Tools3D] Copy from FreeCAD0.21, used while build in linux
  
  -FreeCADAPP
  1.[Application] Support record file version in project file, fix some bugs and change style to hipermos.
  2.[ApplicationPy]Support output log.
  3.[AutoTransaction] Fix bug while opencommand.
  4.[ColorModel] Upgrade to FreeCAD0.21.
  5.[Document] Support temporary undo/redo and recover to specific  undo/redo, fix some bugs.
  6.[DocumentObject] Add some virtual interface used by derivate object.
  7.[DocumentObjectGroup] Sign as uncopyable and unpastable by default.
  8.[DocumentObserver] Add interface to update data while undo/redo.
  9.[DocumentPyImp] Support Find objects with type.
  10.[GeoFeature] Support notify other objects while geometry is changed.
  11.[GeoFeatureGroupExtension] Fix bug of crash.
  12.[GroupExtension]Support insert object while paste.
  13.[Material]Change default diffuse color.
  14.[Property] Fix bug of porps status error.
  15.[PropertyFile] Fix bug while paste.
  16.[PropertyLinks]fix bug of set link list value.
  17.[PropertyStandard]fix bug of object view name while rename.
  18.[TransactionalObject] Support ignore some properties recorded to undo/redo while property value changed.
  19.[Transactions] Fix bugs of undo/redo.

  -FreeCADGUI
  1.[PropertyItem] Fix bug of prop edited.
  2.[Actiongroup] Fix bug of vibrate while expand and fold.
  3.[actionpanel] Unify the scheme for all contents.
  4.[taskheader]Don't allow fold then unfold if press icon button but not release.
  5.[Quarter,SensorManager] Fix bug of crash while update object property in multi thread.
  6.[TaskDialog] Fix bug of crash while close task dialog.
  7.[TaskView] Fix bug of drawer blank after folding.
  8.[Action] Fix bug of retranslate and update project info while open/close document.
  9.[ActionFunction] Add log info while interact.
  10.[Application] Support inheritable and fix some bugs.
  11.[AutoSaver] Support configure the switch of auto saver.
  12.[Command] Support output log info and translate.
  13.[DlgDisplayPropertiesImp] Support undo while change display color.
  14.[DlgEditorImp,DlgReportViewImp,DlgSettingsDocumentImp,DlgSettingsMacroImp,DlgSettingsNavigation,DlgSettingsUnitsImp,
  DlgSettingsViewColor,PropertyPage,WidgetFactory] Support resetting.
  15.[DlgGeneralImp] Hide some parameters and support resetting.
  16.[DlgPreferencesImp] Fix icon size and support resetting.
  17.[DlgPropertyLink] Support record the original selection source, from view or from navigate tree.
  18.[DlgSettings3DViewImp,DlgSettingsColorGradientImp] Change color configure mode and support resetting.
  19.[DlgUndoRedo] Fix bug of changing langeuage .
  20.[DockWindowManager] Fix some bugs.
  21.[Document] Support inheritable and fix some bugs.
  22.[DocumentPyImp] Support set document modified.
  23.[GLPainter] Fix bugs while selection in rectangle mode.
  24.[MainWindow] Support inheritable adn fix some bugs.
  25.[MDIView] Forbid change view while some work is active.
  26.[MouseSelection] Support select hide object while keep mouse button pressed, Fix some bugs.
  27.[NaviCube] Fix bug of translation and forbid some unused command.
  28.[NavigationStyle] Forbid some unused style.
  29.[PrefWidgets] Fix bug of multi notify, which is time consume.
  30.[ProgressBar] Fix bug of show progressbar in multi thread.
  31.[ReportView]Do not show report view by default.
  32.[Selection,TaskElementColors] Support record the source operation of selection and fix some bugs.
  33.[SoAxisCrossKit]Fix bug of axis width change greater while window height is change small.
  34.[SoFCColorBar,SoFCColorGradient,SoFCColorLegend]Upgrade to FreeCAD0.21.
  35.[SoFCSelection] Unify selection logic to SoFCUnifiedSelection.
  36.[SoFCUnifiedSelection] Support Navigate mode and selection mode .
  37.[SoFCSelectionContext] Fix bug of selection by transplant code from SoBrepFace.
  38.[SoTextLabel] Upgrade to FreeCAD0.21.
  39.[SpinBox]Support valid check.
  40.[ToolBarManager] Fix bug of toolbar lost while active workbench.
  41.[TransactionObject] Fix bug while undo/redo.
  42.[View3DInventor] Support inheritable.
  42.[View3DInventorViewer] Support inheritable and fix some bugs.
  43.[View3DPy]fix bug for coordinate selection.
  44.[ViewProvider]don't respond key escape.
  45.[ViewProviderDocumentObject]Support focus show mode and fix bugs of visibility while undo/redo.
  46.[ViewProviderDocumentObjectGroup] Support set group object transparency.
  47.[ViewProviderGeometryObject] Support highlight mode.
  48.[ViewProviderGroupExtension] do not confirm delete.
  49.[Widgets]Fixed bug of geometry tips.
  50.[Workbench]Hide some unneeded command.
  
  -Draft
  1.[DraftDxf,dxf]support 3d arc,circle,ellipse.
  2.[gui_snapper,gui_snaps]Enhanced function fo snapper and fix some bugs.
  
  -Import
  1.[ImpExpDxf]Fix bug of import empty file.
  2.[ImportOCAF2]Set keepPlacement true as default and fix color for export.
  3.[AppImportGuiPy] Fix export model color bug.
  
  
  -Part
  1.[TopoShape]Support create topo shape relationship which is not support by opencascade.
  
  -PartGui
  1.[AppPartGui]Do not show part design parameters in preference widget.
  2.[DlgSettings3DViewPartImp,DlgSettingsGeneral,DlgSettingsObjectColor]Support reset parameter.
  3.[SoBrepEdgeSet]Support show curve which is shaded by part.
  4.[SoBrepFaceSet,SoBrepPointSet]Support show hilight and selection.
  5.[ViewProviderCompound]Fixed bug of object display error during undo while delete compond obj.
  6.[ViewProviderExt]Support select vertex/edge/face by box and fix display tolerance.
  
  -Mesh
  1.[Builder]Fix bug while cancel import mesh.
  2.[Decimation] Update to FreeCAD0.21.
  3.[MeshIO] Fix bug of import model with color and support show progressbar while import big model.
  4.[AppMeshPy] Support import models as whole.
  5.[Exporter]Export the model with the position while export.
  6.[Mesh] Add functions for acquiring face vertex.
  7.[MeshFeature]Support copy/paste.
  
  -MeshGui
  1.[DlgSettingsImportExportImp,DlgSettingsMeshView]Suport reset preference parameter.
  2.[MeshSelection]Support select single facet.
  3.[SoFCIndexedFaceSet] Try to improve display efficiency and memory consume while edit transparency.
  4.[ViewProvider]Fix bug of view mode while change selection.
  5.[ViewProviderMeshFaceSet]Fix bug of display error.
  
  -Sketch
  1.[planegcs,Sketch,SolverGeometryExtension]Update to FreeCAD0.21.
  -SketchGUi
  1.[AppSketcherGui]Do not show sketch parameter in preference widget.
  2.[SketcherSettings,TaskSketcherGeneral]Support reset parameter.
  3.[ViewProviderSketch]Support inheritable.
  
  WebGui
  1.[AppWebGui]Support refresh while some project information updated.
  
  
  