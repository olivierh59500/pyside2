project(QtWidgets)


set(QtWidgets_OPTIONAL_SRC )
set(QtWidgets_DROPPED_ENTRIES )
## gone check_qt_class(Qt5Widgets QAbstractPageSetupDialog   QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
## actually, all the printer stuff is in QtPrintSupport
## XXX check if these conditionals need to be done elsewhere
check_qt_class(Qt5Widgets QAbstractPrintDialog       QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QGtkStyle                  QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QPageSetupDialog           QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QPrintDialog               QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QPrintEngine               QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QPrintPreviewDialog        QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QPrintPreviewWidget        QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QPrinter                   QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QPrinterInfo               QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QSessionManager            QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QSizeGrip                  QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QSystemTrayIcon            QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)
check_qt_class(Qt5Widgets QMacStyle                  QtWidgets_OPTIONAL_SRC QtWidgets_DROPPED_ENTRIES)

set(QtWidgets_SRC
${QtWidgets_GEN_DIR}/qabstractbutton_wrapper.cpp
${QtWidgets_GEN_DIR}/qabstractgraphicsshapeitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qabstractitemdelegate_wrapper.cpp
${QtWidgets_GEN_DIR}/qabstractitemview_wrapper.cpp
${QtWidgets_GEN_DIR}/qabstractscrollarea_wrapper.cpp
${QtWidgets_GEN_DIR}/qabstractslider_wrapper.cpp
${QtWidgets_GEN_DIR}/qabstractspinbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qaction_wrapper.cpp
${QtWidgets_GEN_DIR}/qactiongroup_wrapper.cpp
${QtWidgets_GEN_DIR}/qapplication_wrapper.cpp
${QtWidgets_GEN_DIR}/qboxlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qbuttongroup_wrapper.cpp
${QtWidgets_GEN_DIR}/qcalendarwidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qcheckbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qcolordialog_wrapper.cpp
${QtWidgets_GEN_DIR}/qcolumnview_wrapper.cpp
${QtWidgets_GEN_DIR}/qcombobox_wrapper.cpp
${QtWidgets_GEN_DIR}/qcommandlinkbutton_wrapper.cpp
${QtWidgets_GEN_DIR}/qcommonstyle_wrapper.cpp
${QtWidgets_GEN_DIR}/qcompleter_wrapper.cpp
${QtWidgets_GEN_DIR}/qdatawidgetmapper_wrapper.cpp
${QtWidgets_GEN_DIR}/qdateedit_wrapper.cpp
${QtWidgets_GEN_DIR}/qdatetimeedit_wrapper.cpp
${QtWidgets_GEN_DIR}/qdesktopwidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qdial_wrapper.cpp
${QtWidgets_GEN_DIR}/qdialog_wrapper.cpp
${QtWidgets_GEN_DIR}/qdialogbuttonbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qdirmodel_wrapper.cpp
${QtWidgets_GEN_DIR}/qdockwidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qdoublespinbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qerrormessage_wrapper.cpp
${QtWidgets_GEN_DIR}/qfiledialog_wrapper.cpp
${QtWidgets_GEN_DIR}/qfileiconprovider_wrapper.cpp
${QtWidgets_GEN_DIR}/qfilesystemmodel_wrapper.cpp
${QtWidgets_GEN_DIR}/qfocusframe_wrapper.cpp
${QtWidgets_GEN_DIR}/qfontcombobox_wrapper.cpp
${QtWidgets_GEN_DIR}/qfontdialog_wrapper.cpp
${QtWidgets_GEN_DIR}/qformlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qframe_wrapper.cpp
${QtWidgets_GEN_DIR}/qgesture_wrapper.cpp
${QtWidgets_GEN_DIR}/qgestureevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgesturerecognizer_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsanchor_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsanchorlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsblureffect_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicscolorizeeffect_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsdropshadoweffect_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicseffect_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsellipseitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsgridlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsitemanimation_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsitemgroup_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicslayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicslayoutitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicslinearlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicslineitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsobject_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsopacityeffect_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicspathitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicspixmapitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicspolygonitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsproxywidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsrectitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsrotation_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscale_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscene_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscenecontextmenuevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscenedragdropevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicssceneevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscenehelpevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscenehoverevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscenemouseevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscenemoveevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicssceneresizeevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsscenewheelevent_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicssimpletextitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicstextitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicstransform_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicsview_wrapper.cpp
${QtWidgets_GEN_DIR}/qgraphicswidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qgridlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qgroupbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qhboxlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qheaderview_wrapper.cpp
${QtWidgets_GEN_DIR}/qinputdialog_wrapper.cpp
${QtWidgets_GEN_DIR}/qitemdelegate_wrapper.cpp
${QtWidgets_GEN_DIR}/qitemeditorcreatorbase_wrapper.cpp
${QtWidgets_GEN_DIR}/qitemeditorfactory_wrapper.cpp
${QtWidgets_GEN_DIR}/qkeyeventtransition_wrapper.cpp
${QtWidgets_GEN_DIR}/qlabel_wrapper.cpp
${QtWidgets_GEN_DIR}/qlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qlayoutitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qlcdnumber_wrapper.cpp
${QtWidgets_GEN_DIR}/qlineedit_wrapper.cpp
${QtWidgets_GEN_DIR}/qlistview_wrapper.cpp
${QtWidgets_GEN_DIR}/qlistwidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qlistwidgetitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qmainwindow_wrapper.cpp
${QtWidgets_GEN_DIR}/qmdiarea_wrapper.cpp
${QtWidgets_GEN_DIR}/qmdisubwindow_wrapper.cpp
${QtWidgets_GEN_DIR}/qmenu_wrapper.cpp
${QtWidgets_GEN_DIR}/qmenubar_wrapper.cpp
${QtWidgets_GEN_DIR}/qmessagebox_wrapper.cpp
${QtWidgets_GEN_DIR}/qmouseeventtransition_wrapper.cpp
${QtWidgets_GEN_DIR}/qpangesture_wrapper.cpp
${QtWidgets_GEN_DIR}/qpinchgesture_wrapper.cpp
${QtWidgets_GEN_DIR}/qplaintextdocumentlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qplaintextedit_wrapper.cpp
${QtWidgets_GEN_DIR}/qprogressbar_wrapper.cpp
${QtWidgets_GEN_DIR}/qprogressdialog_wrapper.cpp
${QtWidgets_GEN_DIR}/qpushbutton_wrapper.cpp
${QtWidgets_GEN_DIR}/qradiobutton_wrapper.cpp
${QtWidgets_GEN_DIR}/qrubberband_wrapper.cpp
${QtWidgets_GEN_DIR}/qscrollarea_wrapper.cpp
${QtWidgets_GEN_DIR}/qscrollbar_wrapper.cpp
${QtWidgets_GEN_DIR}/qshortcut_wrapper.cpp
${QtWidgets_GEN_DIR}/qsizegrip_wrapper.cpp
${QtWidgets_GEN_DIR}/qsizepolicy_wrapper.cpp
${QtWidgets_GEN_DIR}/qslider_wrapper.cpp
${QtWidgets_GEN_DIR}/qspaceritem_wrapper.cpp
${QtWidgets_GEN_DIR}/qspinbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qsplashscreen_wrapper.cpp
${QtWidgets_GEN_DIR}/qsplitter_wrapper.cpp
${QtWidgets_GEN_DIR}/qsplitterhandle_wrapper.cpp
${QtWidgets_GEN_DIR}/qstackedlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qstackedwidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qstatusbar_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyle_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleditemdelegate_wrapper.cpp
${QtWidgets_GEN_DIR}/qstylefactory_wrapper.cpp
${QtWidgets_GEN_DIR}/qstylehintreturn_wrapper.cpp
${QtWidgets_GEN_DIR}/qstylehintreturnmask_wrapper.cpp
${QtWidgets_GEN_DIR}/qstylehintreturnvariant_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoption_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionbutton_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptioncombobox_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptioncomplex_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiondockwidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionfocusrect_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionframe_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiongraphicsitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiongroupbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionheader_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionmenuitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionprogressbar_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionrubberband_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionsizegrip_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionslider_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionspinbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiontab_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiontabbarbase_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiontabwidgetframe_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiontitlebar_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiontoolbar_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiontoolbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptiontoolbutton_wrapper.cpp
${QtWidgets_GEN_DIR}/qstyleoptionviewitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qstylepainter_wrapper.cpp
${QtWidgets_GEN_DIR}/qswipegesture_wrapper.cpp
${QtWidgets_GEN_DIR}/qsystemtrayicon_wrapper.cpp
${QtWidgets_GEN_DIR}/qtabbar_wrapper.cpp
${QtWidgets_GEN_DIR}/qtableview_wrapper.cpp
${QtWidgets_GEN_DIR}/qtablewidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qtablewidgetitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qtablewidgetselectionrange_wrapper.cpp
${QtWidgets_GEN_DIR}/qtabwidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qtapandholdgesture_wrapper.cpp
${QtWidgets_GEN_DIR}/qtapgesture_wrapper.cpp
${QtWidgets_GEN_DIR}/qtextbrowser_wrapper.cpp
${QtWidgets_GEN_DIR}/qtextedit_extraselection_wrapper.cpp
${QtWidgets_GEN_DIR}/qtextedit_wrapper.cpp
${QtWidgets_GEN_DIR}/qtilerules_wrapper.cpp
${QtWidgets_GEN_DIR}/qtimeedit_wrapper.cpp
${QtWidgets_GEN_DIR}/qtoolbar_wrapper.cpp
${QtWidgets_GEN_DIR}/qtoolbox_wrapper.cpp
${QtWidgets_GEN_DIR}/qtoolbutton_wrapper.cpp
${QtWidgets_GEN_DIR}/qtooltip_wrapper.cpp
${QtWidgets_GEN_DIR}/qtreeview_wrapper.cpp
${QtWidgets_GEN_DIR}/qtreewidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qtreewidgetitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qtreewidgetitemiterator_wrapper.cpp
${QtWidgets_GEN_DIR}/qundocommand_wrapper.cpp
${QtWidgets_GEN_DIR}/qundogroup_wrapper.cpp
${QtWidgets_GEN_DIR}/qundostack_wrapper.cpp
${QtWidgets_GEN_DIR}/qundoview_wrapper.cpp
${QtWidgets_GEN_DIR}/qvboxlayout_wrapper.cpp
${QtWidgets_GEN_DIR}/qwhatsthis_wrapper.cpp
${QtWidgets_GEN_DIR}/qwidget_wrapper.cpp
${QtWidgets_GEN_DIR}/qwidgetaction_wrapper.cpp
${QtWidgets_GEN_DIR}/qwidgetitem_wrapper.cpp
${QtWidgets_GEN_DIR}/qwizard_wrapper.cpp
${QtWidgets_GEN_DIR}/qwizardpage_wrapper.cpp

${SPECIFIC_OS_FILES}
# module is always needed
${QtWidgets_GEN_DIR}/qtwidgets_module_wrapper.cpp
)

configure_file("${QtWidgets_SOURCE_DIR}/typesystem_widgets.xml.in"
               "${QtWidgets_BINARY_DIR}/typesystem_widgets.xml" @ONLY)

make_path(QtWidgets_typesystem_path ${QtCore_SOURCE_DIR} ${QtGui_SOURCE_DIR}
                                    ${QtCore_BINARY_DIR} ${QtGui_BINARY_DIR}
                                    ${QtWidgets_SOURCE_DIR})

set(QtWidgets_include_dirs  ${QtWidgets_SOURCE_DIR}
                            ${QtWidgets_BINARY_DIR}
                            ${pyside2_SOURCE_DIR}
                            ${Qt5Core_INCLUDE_DIRS}
                            ${Qt5Gui_INCLUDE_DIRS}
                            ${Qt5Widgets_INCLUDE_DIRS}
                            ${SHIBOKEN_INCLUDE_DIR}
                            ${libpyside_SOURCE_DIR}
                            ${SHIBOKEN_PYTHON_INCLUDE_DIR}
                            ${QtCore_GEN_DIR}
                            ${QtGui_GEN_DIR}
                            )
set(QtWidgets_libraries pyside2
                        ${SHIBOKEN_PYTHON_LIBRARIES}
                        ${SHIBOKEN_LIBRARY}
                        ${Qt5Core_LIBRARIES}
                        ${Qt5Gui_LIBRARIES}
                        ${Qt5Widgets_LIBRARIES}
                        )
set(QtWidgets_deps QtGui)

create_pyside_module(QtWidgets
                     QtWidgets_include_dirs
                     QtWidgets_libraries
                     QtWidgets_deps
                     QtWidgets_typesystem_path
                     QtWidgets_SRC
                     ""
                     ${QtWidgets_BINARY_DIR}/typesystem_widgets.xml)
