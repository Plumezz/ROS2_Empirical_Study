# data file
Initially, we collect all ROS2 Humble version packages list from the https://index.ros.org/?search_packages=true#humble. 

All original information collected is shown in all_pkg_info.

rosPkg_humble_version_new.txt, package list.

repository_humble_version_new.txt, repository and its inner packages.

pkgDeps_humble_version_new.txt, the dpendencies of each package.

pkgInfo_humble_version_new.txt, detailed information of each package.

## background data

### build type
The collected build types of all packages are shown in background/build_type_summary.txt.
### test type
Packages with unit test or lint test are shown in background/test_type_pkg.txt and background/lint_pkg_list.txt.


## RQ1

### ros2 project scales

Project scale is collected and shown RQ1/inros2_repo_stats.csv.

### update frequency

The latest update date is 2025-08-29 for analysis and the detailed file is RQ1/pkgInfo_change_humble_version.txt. The summary file is RQ1/date.txt.

## RQ2

### information_error
For the dependent moveit_msgs with ros2 branch, moveit2 with humble branch built failed. After changing the ros2 branch to humble branch of moveit_msgs, moveit2 could build successfully.
The failure log is shown in RQ2/information_error/. Specially, the package moveit_servo failed.

### missing_static_dependencies
The original and fixed log of franka_ros2 are shown in RQ2/missing_static_dependencies

### missing files error

The failure log is shown in RQ2/missing_files_error

### README file error
The related issue is adi_3dtof_image_stitching#12


### reference error
The original and fixed log of libhri are shown in RQ2/reference_error


### repro build
The logs of unreproducible build repositories are shown in RQ2/repro_build 



## RQ3

The CI and test configuration.

### CI repositories
The repositories list with CI configuration is shown in RQ3/have_ci_repos/ci_total_repos.

Core humble repositories list with CI configuration is shown in RQ3/have_ci_repos/ci_humble_repos.

Community repositories list with CI configuration is shown in RQ3/have_ci_repos/ci_ws_repos.


### CI with full workflow include lint
The repositories list  with CI full workflow include lint is shown in RQ3/total_ci_workflow/ci_lint_repos.

Core humble repositories list with CI full workflow include lint is shown in RQ3/total_ci_workflow/ci_lint_repos_humble.

Community repositories list with CI full workflow include lint is shown in RQ3/total_ci_workflow/ci_lint_repos_ws.


### Have test pkgs
The packages list with tests is shown in RQ3/have_test_pkgs/test_pkg_list.

Core humble packages list with tests is shown in RQ3/have_test_pkgs/humble_core_test_pkg_list.

Community packages list with tests is shown in RQ3/have_test_pkgs/community_test_pkg_list.

### Have lint test pkgs
The packages list with lint tests is shown in RQ3/have_lint_test_pkgs/lint_pkg_list.


### Have both CI and test repositorie
The repositories list with both CI and test configuration is shown in RQ3/have_ci_and_test_repos/ci_and_test_total_repos.

Core humble repositories list with both CI and test configuration is shown in RQ3/have_ci_and_test_repos/ci_and_test_humble_repos.

Community repositories list with both CI and test configuration is shown in RQ3/have_ci_and_test_repos/ci_and_test_ws_repos.

### Have unit test packages
The packages list with unit test is shown in RQ3/have_unit_test_pkgs/unit_test_pkg.txt. And unit test errors is shown in RQ3/test_result/unit_test.


### Have lint errors packages
The lint test errors of community packagess are shown in RQ3/test_result/lint_errors/lint_errors.txt.

The lint test errors of humble core packagess are shown in RQ3/test_result/lint_errors/lint_errors.txt.

### lint error counts

The packages with lint errors are shown in RQ3/test_result/lint_errors/lint_errors_pkg_list.txt.

### missing dependencies
The related issue is crazyswarm2#745

### out date

The related issue is shown in RQ3/test_result/out-date.

### redundant dependencies

The related issue is shown in RQ3/redundant_dependencies.


### other test options 
The related pkg is shown in RQ3/other_test_options.
