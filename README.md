# Face Recognition Sign In Wechat Miniprogram

This project is written without systematic learning of HTML5, CSS3, JavaScript and ES6, causing the project structure and code style confusing. Please be careful.

## Progress

| Date      | Progress                                                                                                                                                  |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2019/5/25 | Students can upload photos to the cloud server, then get the charm value combined with face information detection and analysis provided by Tencent cloud. |
| 2019/5/26 | Admin can create student table and check if a table exists according to table's name or id.                                                               |
| 2019/5/27 | Students can login.                                                                                                                                       |
| 2019/5/28 | Students can upload image to the table.                                                                                                                   |
| 2019/5/30 | Solving the problem of unable to upload student id and name.                                                                                              |
| 2019/6/2  | Detect if a student is in the student table based on his or her face.                                                                                     |
| 2019/6/3  | Fix the bug that students can upload multiple faces.                                                                                                      |
| 2019/6/7  | All down.                                                                                                                                                 |

## Problems Encountered and Solved

| Date      | Problems                                                                                                                        |
| --------- | ------------------------------------------------------------------------------------------------------------------------------- |
| 2019/5/25 | After deleting cloud function at the cloud function console, you need to sync the cloud function if you modify it then.         |
| 2019/5/28 | After call `wx.chooseImage()`, attribute `tempFilePath` of `res` in call back fucntion `object.success()`'s is not image or url |
| 2019.5.29 | Cloud functions don't need prefix `wx.` Cloud functions don't have access yto variable inside app.js                            |
| 2019.5.30 | After reset or checkout, remember to upload cloud functions being affected.                                                     |
