# Automated-Digital-Scanner / 3D Printer
A digital scanner/printer that can streamline all of the processes involved to make it simpler for an end-user.

We wanted to create an affordable and simple to use 3 dimensional scanner and printer all-in-one device, one that could potentially help get the non-technical creative user into the 3D modeling field.



1: When most people see a 3D printer demo their typical reaction is excitement, but due to the expertise required in CAD or 3D modeling software it can seem intimidating. Being able to scan an existing object into a model editor where they can then make adjustments is a good way for beginners to get started. 



2. There are many applications for 3D scanning, to name a few:

-	Photo-realistic assets for software such as game or design engines (Unity, Unreal Engine etc)
-	Quick and easy scans of products that can show complete 360 degrees of  rotation the product to the consumer.
-	Seamless transition from scanner to printer.
-	Rapid prototyping.
-	Information repositories or visual archival purposes



3. A Cartesian 3D printer is usually a collection of motors powered by a logic board, we thought it would make sense to simply attach a camera (phone or DSLR) to the X axis of an existing printer. We then attempted to automate the process as much as possible so that it would be easier for a consumer. The ideal use would go as follows:
	
-	Place the object on the turntable
-	Start the scan, the camera would synchronize with the printer host and take time-lapsed pictures as the object spins
-	After the scan, the pictures (RAW) are imported from the camera on to a computer or cloud service.
-	Photogrammetry software creates a dense point cloud from the images, a texture can be baked in as well providing a high quality color scan after a short period of time.
-	The scan could then be imported into a 3D modeling program, or printed as-is with minimal post editing.



4. Shortcomings:

-	We were unable to get the printer host software to talk to the camera, we had to manually initiate the time lapse as the model moves in front of the camera.
-	 We were short on stepper motor drivers and had to sacrifice the Y axis motor in order to run the turntable. Because of this we are not able to print with the camera rigged on.
-	Initially we wanted to use a cloud platform such as Azure to host the RAW photos, but we did not have the time to figure out how to automate the upload from the DSLR
-	Using a smart phone would have been ideal from a consumer standpoint, not everyone will have a DSLR available. A DSLR was easier to get working within the 24 hour time limit.
-	Finally, we wanted to mount the camera to the front of the extruder and use the filament gear to tilt the camera axis by 30 degrees. As the Z axis moves up the camera will move off of the object, automating this would have greatly reduced manual intervention.
-	
+   Copyright 2015 Justin Vorel and Colin Tucker
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+ limitations under the License.
