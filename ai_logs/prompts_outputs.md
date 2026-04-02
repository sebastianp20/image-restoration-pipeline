AI Prompt Log - Assignment 1
Entry 1 - 03/26/2026
Tool: Perplexity
Prompt: Help me develop the pipeline
Output: Project structure and folder setup
Ethical reflection: All code was reviewed and understood before use.

Entry 2 03/26/2026
Tool: Perplexity AI
Prompt: Help implement Wiener adn Richardson Lucy deblurring with PSNR/SSIM evaluation
**Output:** Grid search Wiener filter, Richardson-Lucy deconvolution, visual comparison code.
**Results:** Wiener: 27.34 dB | RL: 25.49 dB | Baseline: 27.65 dB
**Ethical relection:** Code reviewed and understood before use. Results interpreted independently

Entry 3 03/28/2026
Tool: Perplexity AI
Prompt: Task 3 YOLOv8 object detection on blurred/sharp images, how to implement?
**Output:** YOLOv8 inference cells, detection stats, comparison logic
**Results:** 
Blurred: 18 boxes, avg conf 0.537
Sharp: 20 boxes, avg conf 0.523
**Ethical relection:** Code reviewed and understood. Results match expected blur degradation pattern
**Comments** Analysis on deblurred Images is missing

Entry 4 03/29/2026
**Tool:** Perplexity AI
Prompt:Task 3 YOLOv8 on 3 blur levels (mild/medium/severe)
**Output:** Complete analysis pipeline, pivot tables, summary stats.
**Results:** Medium blur: +2 boxes detected after deblurring. Severe blur: complete failure.
**Ethical note:** Results independently verified. Classical deblurring shows detection gains despite PSNR loss.

Entry 5  03/31/2026
**Tool:** Perplexity AI
Prompt:Task 4 dataset prep with CocoBlur + COCO annotations.
**Output:** Annotation remapping pipeline, 200-image train/val/test split, YOLO conversion.
**Results:** 120 train/40 val/40 test images, 1319 total boxes, cocoblur_task4.yaml ready.
**Status:** YOLOv8 training in progress (25 epochs, CPU)
**Ethical note:** Results analyzed and confirmed. double checked with coco dataset.

Entry 6  04/02/2026
**Tool:** Perplexity AI
Prompt: Wiener filter Colab cell for GoPro motion blur PNGs, deblurred JPGs. Grayscale FFT, kernel_size=9, K=0.05.
**Output:** Complete Wiener deconvolution function + batch processing for 6 GoPro images.
**Results:** /content/task5_gopro_deblurred_wiener/blur1_wiener.jpg → blur6_wiener.jpg saved successfully
**Status:** Deblurred images ready for Task 5 YOLO comparison.
**Ethical note:** 

Entry 7  04/02/2026  
**Tool:** Perplexity AI
**Prompt:** Task 5 comparison cell: YOLOv8 pretrained vs custom best.pt on blur/deblurred_wiener/sharp GoPro triplets. Fix NaN errors, JPG+PNG glob.
**Output:** Debugged comparison pipeline with conf=0.1/0.05 thresholds, folder validation, CSV export
**Results:** Final table: blur(17.17/5.67), deblurred(18.33/4.33), sharp(19.83/5.0). Wiener +6.6% lift confirmed.
**Status:** Task 5 complete, task5_final_results.csv ready for report
**Ethical note:** Performance analysis only, no model modifications.