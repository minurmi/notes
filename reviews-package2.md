Usability
Approved with the following notes:
- The ower, author etc. could have roles as every other document.
- Tests could list the following usability related DIRS as well: AINO-DIR-008 "The wrist device shall be rechargeable", AINO-DIR-011 "The wrist device shall indicate whether it's being charged or not", AINO-DIR-078 "User shall be notified that ECG measurement has started [...]"

Algo
- Document name should be AinoECG WD SW PPG Algorithm
- Besides determining "when the user has an arrhythmia episode" doesn't the algorithm detect and classify the beats (AINO-DIR-030 and AINO-DIR-076)? That could be added to the intro and purpose.
- Storage location of SFS-EN 62304/A1:2015 in section 3. could be "Sharepoint, as PODMS-1562054706-19."
- PODMS-1763928776-19 – Algorithm Description should be renamed and approved if that is referred here.
- The "units" (activity, HR, arrhythmia) of the PPG Algorithm "item" should be listed more clearly, e.g. in section 5.1.
- The color coding of the figures could be explained in Figure 1 caption.
- Wouldn't AINO-DIR-035 and AINO-DIR-076 be relevant in the algorithm design?
- Regarding AINO-DIR-038 it should be metioned that the algo produced the trigger to display the notification.
- The document should describe the Algorithm API more clearly. It should include something like these: (IEC 62304 $5.3.2) a) List the main functions b) What does it require from other components? c) How is it supposed to interact with other software? d) (a)synchronous?
- The document should list the functional and performance requirements for the SOUP item that are necessary for its intended use (IEC 62304 $5.3.3, $5.3.4). SOUP: ARM CMIS DSP library for Cortex-M. Functional requirements: arm_cos_f32, arm_sin_f32, arm_sqrt_f32. Performance requirements: XXX


Run on the selected Nordic Semiconductor Cortex-M4 MCU.


Connectivity:
- I would remove Android/smartphone from section 5 (and perhaps from the whole document) and add gateway/Linux
- 7.1.17, 7.2 Product name should be "PulseOn AM-1"
- Appendix A: Add reference to AINO-DIR-070 and AINO-DIR-082. DIRs related to settings (AINO-DIR-032, AINO-DIR-070, AINO-DIR-072, AINO-DIR-082) should refer to Session Control Service and blob since that is the designed way to configure settings in the final product. The settings service is really only used for RnD. Perhaps this info should be made more clear in general.
- Appendix A: Add reference to AINO-DIR-022: The version information service provides a way to retreive this when data is read.
- Appendix A: Add reference to AINO-DIR-028: Data collection parameters are controlled through the session blob, which is practially impossible for patients.

Version info
- Should Appendix A list AINO-DIR-015?
- Does the version info depend on any SOUP such as the nRF5 SDK? I suppose not since the softdevice version is provided via the Bluetooth SW item.

Basic Compression Library
- Add reference to decoder
- rice is a codec that uses the Basic Compression Library to compress/uncompress the data but the encoding and decoding is handled by the rice coded
- I would remove Actana from terms and definitions and refer to the PODMS-1378432600-5837 Aino ECG WD Actana instead.

Scheduled notification will re-trigger arrhythmia alert withing 5 minutes.

Beat Algo
- Do you agree with the term "hear rate state", Antti?
- Make it more clear that the Beat algo is a decomposable software item.
- Section 1.1: "partially how this information is presented" could be "guidelines of how this information is presented"
- Section 1.2: The Atrial Fibrillation should be Arrhythmia as the Python API calls it? (Antti should confirm this)
- Section 5.1: Beat classifications are not displayed to the doctor
- API: Describe the how one day estimate can be derived from the 30-min classifications
- OPTIONAL: add an explanation of the term "web service" to refer to the Data Management Service
- Use agreed table format for Appendix B


Aino ECG Wrist device mechanics specification

Approved with the following comments:
- I don't agree with the term definition "wrist device" to include desktop software.
- Section 5. last paragraph has weird formatting.
- The following DIRs should be mentioned in Appendix A: AINO-DIR-030, AINO-DIR-077, AINO-DIR-078, AINO-DIR-038, AINO-DIR-050, AINO-DIR-045, AINO-DIR-065, AINO-DIR-066


Aino ECG UI
- 6.1.2: Remove USB connection state
- 6.1.4: Cooldown does not become active if case of a failed notification.
- 6.2: "60 second" should be 5-minute

Electronics specification
- Remove empty reviewer field
- Start numbering from 1
- Change table 1 font
- Check DIRs


HAL
- Author role: Emgineer
- Direct recipients: Aino software team members
- CC recipients: -
