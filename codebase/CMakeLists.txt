cmake_minimum_required(VERSION 3.6)
project(project4_04)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")


add_library(RBF rbf/pfm.cc rbf/rbfm.cc)

add_executable(cs222_rbftest1 rbf/rbftest1.cc)
target_link_libraries(cs222_rbftest1 RBF)

add_executable(cs222_rbftest2 rbf/rbftest2.cc)
target_link_libraries(cs222_rbftest2 RBF)

add_executable(cs222_rbftest3 rbf/rbftest3.cc)
target_link_libraries(cs222_rbftest3 RBF)

add_executable(cs222_rbftest4 rbf/rbftest4.cc)
target_link_libraries(cs222_rbftest4 RBF)

add_executable(cs222_rbftest5 rbf/rbftest5.cc)
target_link_libraries(cs222_rbftest5 RBF)

add_executable(cs222_rbftest6 rbf/rbftest6.cc)
target_link_libraries(cs222_rbftest6 RBF)

add_executable(cs222_rbftest8 rbf/rbftest8.cc)
target_link_libraries(cs222_rbftest8 RBF)

add_executable(cs222_rbftest7 rbf/rbftest7.cc)
target_link_libraries(cs222_rbftest7 RBF)

add_executable(cs222_rbftest8b rbf/rbftest8b.cc)
target_link_libraries(cs222_rbftest8b RBF)

add_executable(cs222_rbftest9 rbf/rbftest9.cc)
target_link_libraries(cs222_rbftest9 RBF)

add_executable(cs222_rbftest10 rbf/rbftest10.cc)
target_link_libraries(cs222_rbftest10 RBF)

add_executable(cs222_rbftest11 rbf/rbftest11.cc)
target_link_libraries(cs222_rbftest10 RBF)

add_executable(cs222_rbftest12 rbf/rbftest12.cc)
target_link_libraries(cs222_rbftest10 RBF)

add_executable(mytest rbf/MyTest.cc)
target_link_libraries(mytest RBF)




#
#set(SOURCE_FILES
#    codebase/cli/cli.cc
#    codebase/cli/cli.h
#    codebase/cli/cli_example_01.cc
#    codebase/cli/cli_example_02.cc
#    codebase/cli/cli_example_03.cc
#    codebase/cli/cli_example_04.cc
#    codebase/cli/cli_example_05.cc
#    codebase/cli/cli_example_06.cc
#    codebase/cli/cli_example_07.cc
#    codebase/cli/cli_example_08.cc
#    codebase/cli/cli_example_09.cc
#    codebase/cli/cli_example_10.cc
#    codebase/cli/cli_example_11.cc
#    codebase/cli/cli_example_12.cc
#    codebase/cli/start.cc
#    codebase/ix/ix.cc
#    codebase/ix/ix.h
#    codebase/ix/ix_test_util.h
#    codebase/ix/ixtest_01.cc
#    codebase/ix/ixtest_02.cc
#    codebase/ix/ixtest_03.cc
#    codebase/ix/ixtest_04.cc
#    codebase/ix/ixtest_05.cc
#    codebase/ix/ixtest_06.cc
#    codebase/ix/ixtest_07.cc
#    codebase/ix/ixtest_08.cc
#    codebase/ix/ixtest_09.cc
#    codebase/ix/ixtest_10.cc
#    codebase/ix/ixtest_11.cc
#    codebase/ix/ixtest_12.cc
#    codebase/ix/ixtest_13.cc
#    codebase/ix/ixtest_14.cc
#    codebase/ix/ixtest_15.cc
#    codebase/ix/ixtest_extra_01.cc
#    codebase/ix/ixtest_extra_02.cc
#    codebase/ix/ixtest_p1.cc
#    codebase/ix/ixtest_p2.cc
#    codebase/ix/ixtest_p3.cc
#    codebase/ix/ixtest_p4.cc
#    codebase/ix/ixtest_p5.cc
#    codebase/ix/ixtest_p6.cc
#    codebase/ix/ixtest_pe_01.cc
#    codebase/ix/ixtest_pe_02.cc
#    codebase/qe/qe.cc
#    codebase/qe/qe.h
#    codebase/qe/qe_test_util.h
#    codebase/qe/qetest_01.cc
#    codebase/qe/qetest_02.cc
#    codebase/qe/qetest_03.cc
#    codebase/qe/qetest_04.cc
#    codebase/qe/qetest_05.cc
#    codebase/qe/qetest_06.cc
#    codebase/qe/qetest_07.cc
#    codebase/qe/qetest_08.cc
#    codebase/qe/qetest_09.cc
#    codebase/qe/qetest_10.cc
#    codebase/qe/qetest_11.cc
#    codebase/qe/qetest_12.cc
#    codebase/qe/qetest_13.cc
#    codebase/qe/qetest_14.cc
#    codebase/qe/qetest_15.cc
#    codebase/qe/qetest_16.cc
#    codebase/rbf/pfm.cc
#    codebase/rbf/pfm.h
#    codebase/rbf/rbfm.cc
#    codebase/rbf/rbfm.h
#    codebase/rbf/rbftest1.cc
#    codebase/rbf/rbftest10.cc
#    codebase/rbf/rbftest11.cc
#    codebase/rbf/rbftest12.cc
#    codebase/rbf/rbftest2.cc
#    codebase/rbf/rbftest3.cc
#    codebase/rbf/rbftest4.cc
#    codebase/rbf/rbftest5.cc
#    codebase/rbf/rbftest6.cc
#    codebase/rbf/rbftest7.cc
#    codebase/rbf/rbftest8.cc
#    codebase/rbf/rbftest8b.cc
#    codebase/rbf/rbftest9.cc
#    codebase/rbf/test_util.h
#    codebase/rm/rm.cc
#    codebase/rm/rm.h
#    codebase/rm/rm_test_util.h
#    codebase/rm/rmtest_00.cc
#    codebase/rm/rmtest_01.cc
#    codebase/rm/rmtest_02.cc
#    codebase/rm/rmtest_03.cc
#    codebase/rm/rmtest_04.cc
#    codebase/rm/rmtest_05.cc
#    codebase/rm/rmtest_06.cc
#    codebase/rm/rmtest_07.cc
#    codebase/rm/rmtest_08.cc
#    codebase/rm/rmtest_09.cc
#    codebase/rm/rmtest_10.cc
#    codebase/rm/rmtest_11.cc
#    codebase/rm/rmtest_12.cc
#    codebase/rm/rmtest_13.cc
#    codebase/rm/rmtest_13b.cc
#    codebase/rm/rmtest_14.cc
#    codebase/rm/rmtest_15.cc
#    codebase/rm/rmtest_create_tables.cc
#    codebase/rm/rmtest_delete_tables.cc
#    codebase/rm/rmtest_extra_1.cc
#    codebase/rm/rmtest_extra_2.cc
#    codebase/rm/rmtest_p0.cc
#    codebase/rm/rmtest_p1.cc
#    codebase/rm/rmtest_p2.cc
#    codebase/rm/rmtest_p3.cc
#    codebase/rm/rmtest_p4.cc
#    codebase/rm/rmtest_p5.cc
#    codebase/rm/rmtest_p6.cc
#    codebase/rm/rmtest_p7.cc
#    codebase/rm/rmtest_p8.cc
#    codebase/rm/rmtest_p9.cc
#    codebase/rm/rmtest_pex1.cc
#    codebase/rm/rmtest_pex2.cc
#    codebase/shared.h)
#
#add_executable(project4_04 ${SOURCE_FILES})