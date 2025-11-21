<!--- Provide a general summary of your changes in the Title above -->
<!--- Format: [TYPE] Brief description (e.g., [FIX] Motor controller timeout, [FEAT] Add YOLOv8 detection) -->

## Description:
<!--- Describe your changes in detail -->
<!--- What does this PR do and why is it needed? -->

## Related Issue:
<!--- Link to the issue here: Closes #123, Relates to #456 -->
<!--- If suggesting a new feature or change, please discuss it in an issue first -->
<!--- If fixing a bug, there should be an issue describing it with steps to reproduce -->

## Type of Change:
<!--- Check what applies -->
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Configuration/Infrastructure (Ansible, Docker, CI/CD, build systems)
- [ ] Refactoring (no functional changes)
- [ ] Performance improvement

## How Has This Been Tested?
<!--- BE SPECIFIC - describe your testing environment and methodology -->

### Testing Status:
- [ ] Robot tested (full integration on actual robot)
- [ ] Bench tested (hardware components/modules tested on table)
- [ ] Locally verified (script/playbook/model runs as expected on dev machine)
- [ ] Simulation tested (Gazebo/RViz/MATLAB Simulink/custom sim)
- [ ] Builds successfully but not functionally tested yet (explain reason below)

### Testing Details:
<!--- Describe what you tested and results -->
<!--- For embedded/firmware: MCU/board used, Flash/RAM impact, sensor readings, CAN bus tested -->
<!--- For ROS: Nodes tested, topics/services verified, TF tree checked, controllers tested -->
<!--- For perception/CV: Dataset used, model accuracy, inference time, lighting conditions -->
<!--- For MATLAB/Simulink: Model validated, simulation parameters, results -->
<!--- For Ansible/Docker: Target systems, dry run results, idempotency verified, containers tested -->
<!--- For web/GUI: Browser tested, responsiveness, API endpoints verified -->
<!--- For bench testing: Which components/modules, test duration, parameters tested -->

## Screenshots/Evidence (if appropriate):
<!--- HIGHLY RECOMMENDED: Terminal output, plots, videos, oscilloscope captures -->
<!--- For ROS: rqt_graph, RViz screenshots, rosbag info -->
<!--- For perception: detection/segmentation results, confusion matrix -->
<!--- For embedded: serial monitor logs, CAN bus traces -->
<!--- For web/GUI: screenshots of UI, network tab showing API calls -->

## Breaking Changes & Migration:
<!--- Does this PR break existing code that teammates are using? -->
<!--- Breaking change = other people need to modify their code for it to work with your changes -->
<!--- Examples: -->
<!---   - Updated CAN library API: motor_init() now requires speed parameter -->
<!---   - Removed ROS topic /cmd_vel, replaced with /robot/velocity -->
<!---   - Changed config file format from JSON to YAML -->
<!---   - Modified function signature: setSpeed(int) -> setSpeed(int, bool direction) -->
<!---   - Renamed perception class DetectionNode -> ObjectDetector -->
<!--- If NO breaking changes: Just leave this section blank -->

**What breaks:** 
<!-- Describe what existing code/configs will stop working -->
<!-- Example: "motor_init() function now requires speed parameter - old code calling motor_init() will fail to compile" -->
<!-- OR just write "None" -->

**How to fix it:**
<!-- Tell teammates exactly what they need to change in their code -->
<!-- Example: "Update all motor_init() calls to motor_init(50) where 50 is desired speed" -->
<!-- OR write "N/A" if no breaking changes -->

## Checklist (Assignee):
- [ ] PR tackles a single feature/issue (not mixing multiple unrelated changes)
- [ ] No unnecessary changes unrelated to this PR
- [ ] Added comments for complex logic, TODOs, non-obvious decisions
- [ ] Code compiles/builds without errors or warnings
- [ ] Tested according to "Testing Status" section above
- [ ] Documentation updated if needed (README, wiki, inline docs)
- [ ] Evidence uploaded (rosbags/videos/screenshots/logs as appropriate)
- [ ] Added correct PR labels (enhancement, bug, embedded, ros, perception, ansible, docker, matlab, web, etc.)
- [ ] No commented code blocks (use git history instead)
- [ ] Code follows team style guide and naming conventions

## Checklist (Reviewer):
- [ ] Verified all Assignee checks above
- [ ] Code is well-organized, readable, and follows team standards
- [ ] Documentation is clear and sufficient
- [ ] Testing evidence reviewed (rosbags/videos/logs match claimed behavior)
- [ ] Changes tested/verified according to "Testing Status" section
- [ ] No obvious bugs, edge cases, or safety issues
- [ ] For infrastructure/deployment changes: rollback procedure is safe and clear