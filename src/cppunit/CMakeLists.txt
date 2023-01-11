# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
# Name:        3rdparty/cppunit/CMakeLists.txt
# Project:     CppUnit: Unit test library
# Author:      Nick Matthews (This file only)
# Website:     https://github.com/Ultimaker/CppUnit
# Created:     9th January 2023
# Copyright:   Copyright (c) 2023, Nick Matthews.
# Licence:     LGPL-2.1
# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #

set( CPPUNIT_FILES
    AdditionalMessage.cpp
    Asserter.cpp
    BriefTestProgressListener.cpp
    CompilerOutputter.cpp
    DefaultProtector.cpp
    #DllMain.cpp #Apparently this one isn't built.
    DynamicLibraryManager.cpp
    DynamicLibraryManagerException.cpp
    Exception.cpp
    Message.cpp
    PlugInManager.cpp
    PlugInParameters.cpp
    Protector.cpp
    ProtectorChain.cpp
    RepeatedTest.cpp
    ShlDynamicLibraryManager.cpp
    SourceLine.cpp
    StringTools.cpp
    SynchronizedObject.cpp
    Test.cpp
    TestAssert.cpp
    TestCase.cpp
    TestCaseDecorator.cpp
    TestComposite.cpp
    TestDecorator.cpp
    TestFactoryRegistry.cpp
    TestFailure.cpp
    TestLeaf.cpp
    TestNamer.cpp
    TestPath.cpp
    TestPlugInDefaultImpl.cpp
    TestResult.cpp
    TestResultCollector.cpp
    TestRunner.cpp
    TestSetUp.cpp
    TestSuccessListener.cpp
    TestSuite.cpp
    TestSuiteBuilderContext.cpp
    TextOutputter.cpp
    TextTestProgressListener.cpp
    TextTestResult.cpp
    TextTestRunner.cpp
    TypeInfoHelper.cpp
    UnixDynamicLibraryManager.cpp
    Win32DynamicLibraryManager.cpp
    XmlDocument.cpp
    XmlElement.cpp
    XmlOutputter.cpp
    XmlOutputterHook.cpp
)

include_directories( ../../include/ )

add_library( cppunit ${CPPUNIT_FILES} )
