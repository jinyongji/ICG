cmake_minimum_required(VERSION 3.10)

add_executable(evaluate_rbot_dataset evaluate_rbot_dataset.cpp rbot_evaluator.cpp)
target_link_libraries(evaluate_rbot_dataset PUBLIC icg)

add_executable(parameter_study_rbot_dataset parameter_study_rbot_dataset.cpp rbot_evaluator.cpp)
target_link_libraries(parameter_study_rbot_dataset PUBLIC icg)

add_executable(evaluate_choi_dataset evaluate_choi_dataset.cpp choi_evaluator.cpp)
target_link_libraries(evaluate_choi_dataset PUBLIC icg)

add_executable(parameter_study_choi_dataset parameter_study_choi_dataset.cpp choi_evaluator.cpp)
target_link_libraries(parameter_study_choi_dataset PUBLIC icg)

add_executable(evaluate_opt_dataset evaluate_opt_dataset.cpp opt_evaluator.cpp)
target_link_libraries(evaluate_opt_dataset PUBLIC icg)

add_executable(parameter_study_opt_dataset parameter_study_opt_dataset.cpp opt_evaluator.cpp)
target_link_libraries(parameter_study_opt_dataset PUBLIC icg)

add_executable(evaluate_ycb_dataset evaluate_ycb_dataset.cpp ycb_evaluator.cpp)
target_link_libraries(evaluate_ycb_dataset PUBLIC icg)

add_executable(parameter_study_ycb_dataset parameter_study_ycb_dataset.cpp ycb_evaluator.cpp)
target_link_libraries(parameter_study_ycb_dataset PUBLIC icg)

add_executable(run_on_recorded_sequence run_on_recorded_sequence.cpp)
target_link_libraries(run_on_recorded_sequence PUBLIC icg)

add_executable(run_generated_tracker run_generated_tracker.cpp)
target_link_libraries(run_generated_tracker PUBLIC icg)

#if (USE_AZURE_KINECT)
    #add_executable(record_camera_sequence record_camera_sequence.cpp)
    #target_link_libraries(record_camera_sequence PUBLIC icg)

    #add_executable(run_on_camera_sequence run_on_camera_sequence.cpp)
   # target_link_libraries(run_on_camera_sequence PUBLIC icg)
#endif ()
