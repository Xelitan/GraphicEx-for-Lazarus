# GraphicEx for Lazarus
Fork of GraphicEx based on https://github.com/Wormnest/graphicex quickly ported to Lazarus/Free Pascal

Licence: Mozilla Public License

## Supported image formats
TIFF images (.tif; .tiff)

    RGB(A), Grayscale(A), Indexed(A), CMYK(A), Lab*(A), YCbCr, ICCLab, ITULab, CIELog2L, CIELog2Luv
    1..64 bits per sample, including 16, 24, 32 and 64 bits floating point
    Uncompressed, packbits, LZW, CCITT T.4, Thunderscan, Deflate, new and old style JPEG, etc.
    Uses libtiff version 4.0.7

Photoshop images (.psd, .pdd)

    RGB(A), Indexed(A), Grayscale(A), CMYK(A), CIE Lab*
    1, 8, 16 bits per sample integer, 32 bits per sample float
    Uncompressed, packbits
    Reads the combined image
    Color profiles can be read and used except for indexed (needs LCMS to be defined)

Paintshop Pro images (.psp)

    RGB(A), Indexed, Grayscale
    1, 4, 8, 16 bits per sample
    Uncompressed, RLE and LZ77

Gimp XCF images (.xcf)

    RGB(A), Indexed(A), Grayscale(A)
    1, 8 bits per sample
    Uncompressed, RLE

Jpeg images (.jpeg, .jpg, .jpe, .jfif)

    RGB, Grayscale, CMYK, YCbCr, YCCk
    8 bits per sample
    Jpeg compression
    Automatic rotation based on Exif orientation tag (can be disabled)
    Color profiles can be read and used (needs LCMS to be defined)
    Uses libjpeg
    Saving support included (24 bits destination only, progressive not supported)

Portable network graphic images (.png)

    RGB(A), Indexed(A), Grayscale(A)
    1, 2, 4, 8, 16 bits per sample
    LZ77 compressed
    Color profiles can be read and used except for interlaced images (needs LCMS to be defined)

Gif images (.gif)

    Indexed
    1, 4, 8 bits per sample
    LZW compressed
    All image frames can be read (but not animated)

Targa Truevision images (.tga; .vst; .icb; .vda; .win)

    24 bits RGB(A)(888), 15 bits RGB (555), Grayscale, Indexed
    5 and 8 bits per sample
    Uncompressed, RLE
    Saving support included

Kodak Photo-CD images (.pcd)

    8 bits per sample in YCbCr in any resolution (192 x 128 up to 6144 x 4096)

Portable pixel/gray/bw map images (.ppm, .pgm, .pbm)

    RGB, Grayscale, B/W
    1..16 bits per sample
    Uncompressed

ZSoft Paintbrush images (.pcx, .pcc)

    RGB, Indexed (including CGA palette images), Grayscale
    1..8 bits per sample
    Uncompressed, RLE
    Also reads obsolete Word for Dos screen capture images that are very similar to pcx (.scr)

GFI fax images (.fax)

    Uses the Tiff image reading class

EPS images (.eps)

    Only .eps images that have embedded pixel graphics in TIF format.

SGI images (.bw, .rgb, .rgba, .sgi)

    RGB(A), Grayscale(A)
    8, 16 bits per sample
    RLE, uncompressed

SGI Alias/Wavefront images (.rla, .rpf)

    RGB(A), Grayscale(A)
    1..16 bits per sample integer, 32 bits per sample float
    RLE compressed, Uncompressed (for float only)

Maya images (.iff)

    RGB(A)
    8 bits per sample
    RLE, Uncompressed

Amiga ilbm and pbm images (.ilbm, .lbm, .pbm, .iff)

    RGB(A), Indexed(A), Ham, Extra HalfBrite, Sham, Ctbl, Rgb8, Rgbn
    1-8 bits per sample; 1-8, 24, 32 planes
    RLE, RGBN RLE, Uncompressed

Dr. Halo images (.cut, .pal)

    Indexed
    8 bits per sample
    RLE compressed

Autodesk Animator images files (.cel; .pic), old style only

    Indexed
    8 bits per sample
    Uncompressed

