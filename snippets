## Εισαγωγή Δεδομένων

Συνδέστε το Google Drive και φορτώστε τα δεδομένα από τον δίσκο για πρόσβαση στα αρχεία dataset.

```python
from google.colab import drive
drive.mount('/content/drive')

### 2. Αποσυμπίεση Δεδομένων
```markdown
## Αποσυμπίεση Δεδομένων

Αποσυμπιέστε το αρχείο ZIP που περιέχει τις σαρώσεις CT.

```python
import zipfile
zip_ref = zipfile.ZipFile('/content/drive/MyDrive/Colab Notebooks/archive.zip', 'r')
zip_ref.extractall('../input/covid19-ct-scans')
zip_ref.close()

### 3. Cropping
```markdown
## Cropping

Εφαρμόζει Cropping στις εικόνες για να προσδιορίσει και να επικεντρωθεί στις σημαντικότερες περιοχές της σάρωσης.

```python
for img_no in range(array.shape[0]):
    img = cv2.resize(array[img_no], dsize=(img_size, img_size), interpolation=cv2.INTER_AREA)
    lung_mask_resized = cv2.resize(lung_mask[img_no], dsize=(img_size, img_size), interpolation=cv2.INTER_NEAREST)

### 4. CLAHE
```markdown
## CLAHE (Contrast Limited Adaptive Histogram Equalization)

Εφαρμογή του CLAHE για βελτίωση της αντίθεσης της εικόνας.

```python
img_8bit = np.uint8(img * 255)
clahe = cv2.createCLAHE(clipLimit=3.0, tileGridSize=(32,32))
clahe_img = clahe.apply(img_8bit)

# Gamma Correction
gamma = 1.2
img = np.array(255 * (clahe_img / 255) ** gamma, dtype='uint8')

### 5. Image Augmentation
```markdown
## Image Augmentation

Εφαρμογή διαφορετικών τεχνικών αύξησης δεδομένων για να αυξηθεί η ποικιλομορφία των δεδομένων και να βελτιωθεί η απόδοση του μοντέλου.

```python
from imgaug import augmenters as iaa

seq = iaa.Sequential([
    iaa.Fliplr(0.5),  # horizontal flips
    iaa.Flipud(0.2),  #

### 5. Image Augmentation
```markdown
## Image Augmentation

Εφαρμογή διαφορετικών τεχνικών αύξησης δεδομένων για να αυξηθεί η ποικιλομορφία των δεδομένων και να βελτιωθεί η απόδοση του μοντέλου.

```python
from imgaug import augmenters as iaa

seq = iaa.Sequential([
    iaa.Fliplr(0.5),  # horizontal flips
    iaa.Flipud(0.2),  # vertical flips
    iaa.Affine(scale=(0.8, 1)),  # scale images
    iaa.Affine(rotate=(-30, 30))  # rotation
], random_order=True)

def augment_images_and_masks(images, masks):
    seq_det = seq.to_deterministic()  # Ensure same augment

### 5. Image Augmentation
```markdown
## Image Augmentation

Εφαρμογή διαφορετικών τεχνικών αύξησης δεδομένων για να αυξηθεί η ποικιλομορφία των δεδομένων και να βελτιωθεί η απόδοση του μοντέλου.

```python
from imgaug import augmenters as iaa

seq = iaa.Sequential([
    iaa.Fliplr(0.5),  # horizontal flips
    iaa.Flipud(0.2),  # vertical flips
    iaa.Affine(scale=(0.8, 1)),  # scale images
    iaa.Affine(rotate=(-30, 30))  # rotation
], random_order=True)

def augment_images_and_masks(images, masks):
    seq_det = seq.to_deterministic()  # Ensure same augmentations for images and masks
    augmented_images = seq_det(images=images)
    augmented_masks = seq_det(images=masks)
    return augmented_images, augmented_masks
