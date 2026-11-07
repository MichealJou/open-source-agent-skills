# com.feilong.lib.compress.archivers.zip

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.compress.archivers.zip.AbstractUnicodeExtraField`

```java
public abstract class com.feilong.lib.compress.archivers.zip.AbstractUnicodeExtraField implements com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public long getNameCRC32();
  public void setNameCRC32(long);
  public byte[] getUnicodeName();
  public void setUnicodeName(byte[]);
  public byte[] getCentralDirectoryData();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.AsiExtraField`

```java
public class com.feilong.lib.compress.archivers.zip.AsiExtraField implements com.feilong.lib.compress.archivers.zip.ZipExtraField,com.feilong.lib.compress.archivers.zip.UnixStat,java.lang.Cloneable {
  public com.feilong.lib.compress.archivers.zip.AsiExtraField();
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public byte[] getCentralDirectoryData();
  public void setUserId(int);
  public int getUserId();
  public void setGroupId(int);
  public int getGroupId();
  public void setLinkedFile(java.lang.String);
  public java.lang.String getLinkedFile();
  public boolean isLink();
  public void setMode(int);
  public int getMode();
  public void setDirectory(boolean);
  public boolean isDirectory();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
  public java.lang.Object clone();
}
```

## `com.feilong.lib.compress.archivers.zip.CharsetAccessor`

```java
public interface com.feilong.lib.compress.archivers.zip.CharsetAccessor {
  public abstract java.nio.charset.Charset getCharset();
}
```

## `com.feilong.lib.compress.archivers.zip.ExtraFieldParsingBehavior`

```java
public interface com.feilong.lib.compress.archivers.zip.ExtraFieldParsingBehavior extends com.feilong.lib.compress.archivers.zip.UnparseableExtraFieldBehavior {
  public abstract com.feilong.lib.compress.archivers.zip.ZipExtraField createExtraField(com.feilong.lib.compress.archivers.zip.ZipShort) throws java.util.zip.ZipException, java.lang.InstantiationException, java.lang.IllegalAccessException;
  public abstract com.feilong.lib.compress.archivers.zip.ZipExtraField fill(com.feilong.lib.compress.archivers.zip.ZipExtraField, byte[], int, int, boolean) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.ExtraFieldUtils`

```java
public class com.feilong.lib.compress.archivers.zip.ExtraFieldUtils {
  public com.feilong.lib.compress.archivers.zip.ExtraFieldUtils();
  public static void register(java.lang.Class<?>);
  public static com.feilong.lib.compress.archivers.zip.ZipExtraField createExtraField(com.feilong.lib.compress.archivers.zip.ZipShort) throws java.lang.InstantiationException, java.lang.IllegalAccessException;
  public static com.feilong.lib.compress.archivers.zip.ZipExtraField createExtraFieldNoDefault(com.feilong.lib.compress.archivers.zip.ZipShort) throws java.lang.InstantiationException, java.lang.IllegalAccessException;
  public static com.feilong.lib.compress.archivers.zip.ZipExtraField[] parse(byte[]) throws java.util.zip.ZipException;
  public static com.feilong.lib.compress.archivers.zip.ZipExtraField[] parse(byte[], boolean) throws java.util.zip.ZipException;
  public static com.feilong.lib.compress.archivers.zip.ZipExtraField[] parse(byte[], boolean, com.feilong.lib.compress.archivers.zip.ExtraFieldUtils$UnparseableExtraField) throws java.util.zip.ZipException;
  public static com.feilong.lib.compress.archivers.zip.ZipExtraField[] parse(byte[], boolean, com.feilong.lib.compress.archivers.zip.ExtraFieldParsingBehavior) throws java.util.zip.ZipException;
  public static byte[] mergeLocalFileDataData(com.feilong.lib.compress.archivers.zip.ZipExtraField[]);
  public static byte[] mergeCentralDirectoryData(com.feilong.lib.compress.archivers.zip.ZipExtraField[]);
  public static com.feilong.lib.compress.archivers.zip.ZipExtraField fillExtraField(com.feilong.lib.compress.archivers.zip.ZipExtraField, byte[], int, int, boolean) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.ExtraFieldUtils$UnparseableExtraField`

```java
public final class com.feilong.lib.compress.archivers.zip.ExtraFieldUtils$UnparseableExtraField implements com.feilong.lib.compress.archivers.zip.UnparseableExtraFieldBehavior {
  public int getKey();
  public com.feilong.lib.compress.archivers.zip.ZipExtraField onUnparseableExtraField(byte[], int, int, boolean, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.GeneralPurposeBit`

```java
public final class com.feilong.lib.compress.archivers.zip.GeneralPurposeBit implements java.lang.Cloneable {
  public com.feilong.lib.compress.archivers.zip.GeneralPurposeBit();
  public boolean usesUTF8ForNames();
  public void useUTF8ForNames(boolean);
  public boolean usesDataDescriptor();
  public void useDataDescriptor(boolean);
  public boolean usesEncryption();
  public void useEncryption(boolean);
  public boolean usesStrongEncryption();
  public void useStrongEncryption(boolean);
  public byte[] encode();
  public void encode(byte[], int);
  public static com.feilong.lib.compress.archivers.zip.GeneralPurposeBit parse(byte[], int);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.Object clone();
}
```

## `com.feilong.lib.compress.archivers.zip.JarMarker`

```java
public final class com.feilong.lib.compress.archivers.zip.JarMarker implements com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public com.feilong.lib.compress.archivers.zip.JarMarker();
  public static com.feilong.lib.compress.archivers.zip.JarMarker getInstance();
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.PKWareExtraHeader`

```java
public abstract class com.feilong.lib.compress.archivers.zip.PKWareExtraHeader implements com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public void setLocalFileDataData(byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public byte[] getLocalFileDataData();
  public void setCentralDirectoryData(byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$EncryptionAlgorithm`

```java
public final class com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$EncryptionAlgorithm extends java.lang.Enum<com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$EncryptionAlgorithm> {
  public static com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$EncryptionAlgorithm[] values();
  public static com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$EncryptionAlgorithm valueOf(java.lang.String);
  public int getCode();
  public static com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$EncryptionAlgorithm getAlgorithmByCode(int);
}
```

## `com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm`

```java
public final class com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm extends java.lang.Enum<com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm> {
  public static com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm[] values();
  public static com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm valueOf(java.lang.String);
  public int getCode();
  public static com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm getAlgorithmByCode(int);
}
```

## `com.feilong.lib.compress.archivers.zip.ResourceAlignmentExtraField`

```java
public class com.feilong.lib.compress.archivers.zip.ResourceAlignmentExtraField implements com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public com.feilong.lib.compress.archivers.zip.ResourceAlignmentExtraField();
  public com.feilong.lib.compress.archivers.zip.ResourceAlignmentExtraField(int);
  public com.feilong.lib.compress.archivers.zip.ResourceAlignmentExtraField(int, boolean);
  public com.feilong.lib.compress.archivers.zip.ResourceAlignmentExtraField(int, boolean, int);
  public short getAlignment();
  public boolean allowMethodChange();
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.ScatterStatistics`

```java
public class com.feilong.lib.compress.archivers.zip.ScatterStatistics {
  public long getCompressionElapsed();
  public long getMergingElapsed();
  public java.lang.String toString();
}
```

## `com.feilong.lib.compress.archivers.zip.StreamCompressor`

```java
public abstract class com.feilong.lib.compress.archivers.zip.StreamCompressor implements java.io.Closeable {
  public long getCrc32();
  public long getBytesRead();
  public long getBytesWrittenForLastEntry();
  public long getTotalBytesWritten();
  public void deflate(java.io.InputStream, int) throws java.io.IOException;
  public void close() throws java.io.IOException;
  public void writeCounted(byte[]) throws java.io.IOException;
  public void writeCounted(byte[], int, int) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.archivers.zip.UnicodeCommentExtraField`

```java
public class com.feilong.lib.compress.archivers.zip.UnicodeCommentExtraField extends com.feilong.lib.compress.archivers.zip.AbstractUnicodeExtraField {
  public com.feilong.lib.compress.archivers.zip.UnicodeCommentExtraField();
  public com.feilong.lib.compress.archivers.zip.UnicodeCommentExtraField(java.lang.String, byte[], int, int);
  public com.feilong.lib.compress.archivers.zip.UnicodeCommentExtraField(java.lang.String, byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
}
```

## `com.feilong.lib.compress.archivers.zip.UnicodePathExtraField`

```java
public class com.feilong.lib.compress.archivers.zip.UnicodePathExtraField extends com.feilong.lib.compress.archivers.zip.AbstractUnicodeExtraField {
  public com.feilong.lib.compress.archivers.zip.UnicodePathExtraField();
  public com.feilong.lib.compress.archivers.zip.UnicodePathExtraField(java.lang.String, byte[], int, int);
  public com.feilong.lib.compress.archivers.zip.UnicodePathExtraField(java.lang.String, byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
}
```

## `com.feilong.lib.compress.archivers.zip.UnparseableExtraFieldBehavior`

```java
public interface com.feilong.lib.compress.archivers.zip.UnparseableExtraFieldBehavior {
  public abstract com.feilong.lib.compress.archivers.zip.ZipExtraField onUnparseableExtraField(byte[], int, int, boolean, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.UnparseableExtraFieldData`

```java
public final class com.feilong.lib.compress.archivers.zip.UnparseableExtraFieldData implements com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public com.feilong.lib.compress.archivers.zip.UnparseableExtraFieldData();
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int);
  public void parseFromCentralDirectoryData(byte[], int, int);
}
```

## `com.feilong.lib.compress.archivers.zip.UnrecognizedExtraField`

```java
public class com.feilong.lib.compress.archivers.zip.UnrecognizedExtraField implements com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public com.feilong.lib.compress.archivers.zip.UnrecognizedExtraField();
  public void setHeaderId(com.feilong.lib.compress.archivers.zip.ZipShort);
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public void setLocalFileDataData(byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public byte[] getLocalFileDataData();
  public void setCentralDirectoryData(byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int);
  public void parseFromCentralDirectoryData(byte[], int, int);
}
```

## `com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException`

```java
public class com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException extends java.util.zip.ZipException {
  public com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException(com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException$Feature, com.feilong.lib.compress.archivers.zip.ZipArchiveEntry);
  public com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException(com.feilong.lib.compress.archivers.zip.ZipMethod, com.feilong.lib.compress.archivers.zip.ZipArchiveEntry);
  public com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException(com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException$Feature);
  public com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException$Feature getFeature();
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry getEntry();
}
```

## `com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException$Feature`

```java
public class com.feilong.lib.compress.archivers.zip.UnsupportedZipFeatureException$Feature implements java.io.Serializable {
  public java.lang.String toString();
}
```

## `com.feilong.lib.compress.archivers.zip.X000A_NTFS`

```java
public class com.feilong.lib.compress.archivers.zip.X000A_NTFS implements com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public com.feilong.lib.compress.archivers.zip.X000A_NTFS();
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger getModifyTime();
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger getAccessTime();
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger getCreateTime();
  public java.util.Date getModifyJavaTime();
  public java.util.Date getAccessJavaTime();
  public java.util.Date getCreateJavaTime();
  public void setModifyTime(com.feilong.lib.compress.archivers.zip.ZipEightByteInteger);
  public void setAccessTime(com.feilong.lib.compress.archivers.zip.ZipEightByteInteger);
  public void setCreateTime(com.feilong.lib.compress.archivers.zip.ZipEightByteInteger);
  public void setModifyJavaTime(java.util.Date);
  public void setAccessJavaTime(java.util.Date);
  public void setCreateJavaTime(java.util.Date);
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.compress.archivers.zip.X0014_X509Certificates`

```java
public class com.feilong.lib.compress.archivers.zip.X0014_X509Certificates extends com.feilong.lib.compress.archivers.zip.PKWareExtraHeader {
  public com.feilong.lib.compress.archivers.zip.X0014_X509Certificates();
}
```

## `com.feilong.lib.compress.archivers.zip.X0015_CertificateIdForFile`

```java
public class com.feilong.lib.compress.archivers.zip.X0015_CertificateIdForFile extends com.feilong.lib.compress.archivers.zip.PKWareExtraHeader {
  public com.feilong.lib.compress.archivers.zip.X0015_CertificateIdForFile();
  public int getRecordCount();
  public com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm getHashAlgorithm();
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.X0016_CertificateIdForCentralDirectory`

```java
public class com.feilong.lib.compress.archivers.zip.X0016_CertificateIdForCentralDirectory extends com.feilong.lib.compress.archivers.zip.PKWareExtraHeader {
  public com.feilong.lib.compress.archivers.zip.X0016_CertificateIdForCentralDirectory();
  public int getRecordCount();
  public com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm getHashAlgorithm();
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.X0017_StrongEncryptionHeader`

```java
public class com.feilong.lib.compress.archivers.zip.X0017_StrongEncryptionHeader extends com.feilong.lib.compress.archivers.zip.PKWareExtraHeader {
  public com.feilong.lib.compress.archivers.zip.X0017_StrongEncryptionHeader();
  public long getRecordCount();
  public com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$HashAlgorithm getHashAlgorithm();
  public com.feilong.lib.compress.archivers.zip.PKWareExtraHeader$EncryptionAlgorithm getEncryptionAlgorithm();
  public void parseCentralDirectoryFormat(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFileFormat(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.X0019_EncryptionRecipientCertificateList`

```java
public class com.feilong.lib.compress.archivers.zip.X0019_EncryptionRecipientCertificateList extends com.feilong.lib.compress.archivers.zip.PKWareExtraHeader {
  public com.feilong.lib.compress.archivers.zip.X0019_EncryptionRecipientCertificateList();
}
```

## `com.feilong.lib.compress.archivers.zip.X5455_ExtendedTimestamp`

```java
public class com.feilong.lib.compress.archivers.zip.X5455_ExtendedTimestamp implements com.feilong.lib.compress.archivers.zip.ZipExtraField,java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.compress.archivers.zip.X5455_ExtendedTimestamp();
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
  public void setFlags(byte);
  public byte getFlags();
  public boolean isBit0_modifyTimePresent();
  public boolean isBit1_accessTimePresent();
  public boolean isBit2_createTimePresent();
  public com.feilong.lib.compress.archivers.zip.ZipLong getModifyTime();
  public com.feilong.lib.compress.archivers.zip.ZipLong getAccessTime();
  public com.feilong.lib.compress.archivers.zip.ZipLong getCreateTime();
  public java.util.Date getModifyJavaTime();
  public java.util.Date getAccessJavaTime();
  public java.util.Date getCreateJavaTime();
  public void setModifyTime(com.feilong.lib.compress.archivers.zip.ZipLong);
  public void setAccessTime(com.feilong.lib.compress.archivers.zip.ZipLong);
  public void setCreateTime(com.feilong.lib.compress.archivers.zip.ZipLong);
  public void setModifyJavaTime(java.util.Date);
  public void setAccessJavaTime(java.util.Date);
  public void setCreateJavaTime(java.util.Date);
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.compress.archivers.zip.X7875_NewUnix`

```java
public class com.feilong.lib.compress.archivers.zip.X7875_NewUnix implements com.feilong.lib.compress.archivers.zip.ZipExtraField,java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.compress.archivers.zip.X7875_NewUnix();
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public long getUID();
  public long getGID();
  public void setUID(long);
  public void setGID(long);
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.compress.archivers.zip.Zip64ExtendedInformationExtraField`

```java
public class com.feilong.lib.compress.archivers.zip.Zip64ExtendedInformationExtraField implements com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public com.feilong.lib.compress.archivers.zip.Zip64ExtendedInformationExtraField();
  public com.feilong.lib.compress.archivers.zip.Zip64ExtendedInformationExtraField(com.feilong.lib.compress.archivers.zip.ZipEightByteInteger, com.feilong.lib.compress.archivers.zip.ZipEightByteInteger);
  public com.feilong.lib.compress.archivers.zip.Zip64ExtendedInformationExtraField(com.feilong.lib.compress.archivers.zip.ZipEightByteInteger, com.feilong.lib.compress.archivers.zip.ZipEightByteInteger, com.feilong.lib.compress.archivers.zip.ZipEightByteInteger, com.feilong.lib.compress.archivers.zip.ZipLong);
  public com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public byte[] getLocalFileDataData();
  public byte[] getCentralDirectoryData();
  public void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
  public void reparseCentralDirectoryData(boolean, boolean, boolean, boolean) throws java.util.zip.ZipException;
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger getSize();
  public void setSize(com.feilong.lib.compress.archivers.zip.ZipEightByteInteger);
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger getCompressedSize();
  public void setCompressedSize(com.feilong.lib.compress.archivers.zip.ZipEightByteInteger);
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger getRelativeHeaderOffset();
  public void setRelativeHeaderOffset(com.feilong.lib.compress.archivers.zip.ZipEightByteInteger);
  public com.feilong.lib.compress.archivers.zip.ZipLong getDiskStartNumber();
  public void setDiskStartNumber(com.feilong.lib.compress.archivers.zip.ZipLong);
}
```

## `com.feilong.lib.compress.archivers.zip.Zip64Mode`

```java
public final class com.feilong.lib.compress.archivers.zip.Zip64Mode extends java.lang.Enum<com.feilong.lib.compress.archivers.zip.Zip64Mode> {
  public static com.feilong.lib.compress.archivers.zip.Zip64Mode[] values();
  public static com.feilong.lib.compress.archivers.zip.Zip64Mode valueOf(java.lang.String);
}
```

## `com.feilong.lib.compress.archivers.zip.Zip64RequiredException`

```java
public class com.feilong.lib.compress.archivers.zip.Zip64RequiredException extends java.util.zip.ZipException {
  public com.feilong.lib.compress.archivers.zip.Zip64RequiredException(java.lang.String);
}
```

## `com.feilong.lib.compress.archivers.zip.ZipArchiveEntry`

```java
public class com.feilong.lib.compress.archivers.zip.ZipArchiveEntry extends java.util.zip.ZipEntry implements com.feilong.lib.compress.archivers.ArchiveEntry,com.feilong.lib.compress.archivers.EntryStreamOffsets {
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry(java.lang.String);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry(java.util.zip.ZipEntry) throws java.util.zip.ZipException;
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry) throws java.util.zip.ZipException;
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry(java.io.File, java.lang.String);
  public java.lang.Object clone();
  public int getMethod();
  public void setMethod(int);
  public int getInternalAttributes();
  public void setInternalAttributes(int);
  public long getExternalAttributes();
  public void setExternalAttributes(long);
  public void setUnixMode(int);
  public int getUnixMode();
  public boolean isUnixSymlink();
  public int getPlatform();
  public void setAlignment(int);
  public void setExtraFields(com.feilong.lib.compress.archivers.zip.ZipExtraField[]);
  public com.feilong.lib.compress.archivers.zip.ZipExtraField[] getExtraFields();
  public com.feilong.lib.compress.archivers.zip.ZipExtraField[] getExtraFields(boolean);
  public com.feilong.lib.compress.archivers.zip.ZipExtraField[] getExtraFields(com.feilong.lib.compress.archivers.zip.ExtraFieldParsingBehavior) throws java.util.zip.ZipException;
  public void addExtraField(com.feilong.lib.compress.archivers.zip.ZipExtraField);
  public void addAsFirstExtraField(com.feilong.lib.compress.archivers.zip.ZipExtraField);
  public void removeExtraField(com.feilong.lib.compress.archivers.zip.ZipShort);
  public void removeUnparseableExtraFieldData();
  public com.feilong.lib.compress.archivers.zip.ZipExtraField getExtraField(com.feilong.lib.compress.archivers.zip.ZipShort);
  public com.feilong.lib.compress.archivers.zip.UnparseableExtraFieldData getUnparseableExtraFieldData();
  public void setExtra(byte[]) throws java.lang.RuntimeException;
  public void setCentralDirectoryExtra(byte[]);
  public byte[] getLocalFileDataExtra();
  public byte[] getCentralDirectoryExtra();
  public java.lang.String getName();
  public boolean isDirectory();
  public long getSize();
  public void setSize(long);
  public byte[] getRawName();
  public long getDataOffset();
  public boolean isStreamContiguous();
  public int hashCode();
  public com.feilong.lib.compress.archivers.zip.GeneralPurposeBit getGeneralPurposeBit();
  public void setGeneralPurposeBit(com.feilong.lib.compress.archivers.zip.GeneralPurposeBit);
  public java.util.Date getLastModifiedDate();
  public boolean equals(java.lang.Object);
  public void setVersionMadeBy(int);
  public void setVersionRequired(int);
  public int getVersionRequired();
  public int getVersionMadeBy();
  public int getRawFlag();
  public void setRawFlag(int);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$NameSource getNameSource();
  public void setNameSource(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$NameSource);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$CommentSource getCommentSource();
  public void setCommentSource(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$CommentSource);
  public long getDiskNumberStart();
  public void setDiskNumberStart(long);
}
```

## `com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$CommentSource`

```java
public final class com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$CommentSource extends java.lang.Enum<com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$CommentSource> {
  public static com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$CommentSource[] values();
  public static com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$CommentSource valueOf(java.lang.String);
}
```

## `com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$ExtraFieldParsingMode`

```java
public class com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$ExtraFieldParsingMode extends java.lang.Enum<com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$ExtraFieldParsingMode> implements com.feilong.lib.compress.archivers.zip.ExtraFieldParsingBehavior {
  public static com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$ExtraFieldParsingMode[] values();
  public static com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$ExtraFieldParsingMode valueOf(java.lang.String);
  public com.feilong.lib.compress.archivers.zip.ZipExtraField onUnparseableExtraField(byte[], int, int, boolean, int) throws java.util.zip.ZipException;
  public com.feilong.lib.compress.archivers.zip.ZipExtraField createExtraField(com.feilong.lib.compress.archivers.zip.ZipShort) throws java.util.zip.ZipException, java.lang.InstantiationException, java.lang.IllegalAccessException;
  public com.feilong.lib.compress.archivers.zip.ZipExtraField fill(com.feilong.lib.compress.archivers.zip.ZipExtraField, byte[], int, int, boolean) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$NameSource`

```java
public final class com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$NameSource extends java.lang.Enum<com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$NameSource> {
  public static com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$NameSource[] values();
  public static com.feilong.lib.compress.archivers.zip.ZipArchiveEntry$NameSource valueOf(java.lang.String);
}
```

## `com.feilong.lib.compress.archivers.zip.ZipArchiveEntryPredicate`

```java
public interface com.feilong.lib.compress.archivers.zip.ZipArchiveEntryPredicate {
  public abstract boolean test(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry);
}
```

## `com.feilong.lib.compress.archivers.zip.ZipArchiveInputStream`

```java
public class com.feilong.lib.compress.archivers.zip.ZipArchiveInputStream extends com.feilong.lib.compress.archivers.ArchiveInputStream implements com.feilong.lib.compress.utils.InputStreamStatistics {
  public com.feilong.lib.compress.archivers.zip.ZipArchiveInputStream(java.io.InputStream);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveInputStream(java.io.InputStream, java.lang.String);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveInputStream(java.io.InputStream, java.lang.String, boolean);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveInputStream(java.io.InputStream, java.lang.String, boolean, boolean);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveInputStream(java.io.InputStream, java.lang.String, boolean, boolean, boolean);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry getNextZipEntry() throws java.io.IOException;
  public com.feilong.lib.compress.archivers.ArchiveEntry getNextEntry() throws java.io.IOException;
  public boolean canReadEntryData(com.feilong.lib.compress.archivers.ArchiveEntry);
  public int read(byte[], int, int) throws java.io.IOException;
  public long getCompressedCount();
  public long getUncompressedCount();
  public void close() throws java.io.IOException;
  public long skip(long) throws java.io.IOException;
  public static boolean matches(byte[], int);
}
```

## `com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream`

```java
public class com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream extends com.feilong.lib.compress.archivers.ArchiveOutputStream {
  public com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream(java.io.OutputStream);
  public com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream(java.io.File) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream(java.io.File, long) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream(java.nio.channels.SeekableByteChannel) throws java.io.IOException;
  public boolean isSeekable();
  public void setEncoding(java.lang.String);
  public java.lang.String getEncoding();
  public void setUseLanguageEncodingFlag(boolean);
  public void setCreateUnicodeExtraFields(com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream$UnicodeExtraFieldPolicy);
  public void setFallbackToUTF8(boolean);
  public void setUseZip64(com.feilong.lib.compress.archivers.zip.Zip64Mode);
  public void finish() throws java.io.IOException;
  public void closeArchiveEntry() throws java.io.IOException;
  public void addRawArchiveEntry(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry, java.io.InputStream) throws java.io.IOException;
  public void putArchiveEntry(com.feilong.lib.compress.archivers.ArchiveEntry) throws java.io.IOException;
  public void setComment(java.lang.String);
  public void setLevel(int);
  public void setMethod(int);
  public boolean canWriteEntryData(com.feilong.lib.compress.archivers.ArchiveEntry);
  public void write(byte[], int, int) throws java.io.IOException;
  public void close() throws java.io.IOException;
  public void flush() throws java.io.IOException;
  public com.feilong.lib.compress.archivers.ArchiveEntry createArchiveEntry(java.io.File, java.lang.String) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream$UnicodeExtraFieldPolicy`

```java
public final class com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream$UnicodeExtraFieldPolicy {
  public java.lang.String toString();
}
```

## `com.feilong.lib.compress.archivers.zip.ZipEightByteInteger`

```java
public final class com.feilong.lib.compress.archivers.zip.ZipEightByteInteger implements java.io.Serializable {
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger(long);
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger(java.math.BigInteger);
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger(byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipEightByteInteger(byte[], int);
  public byte[] getBytes();
  public long getLongValue();
  public java.math.BigInteger getValue();
  public static byte[] getBytes(long);
  public static byte[] getBytes(java.math.BigInteger);
  public static long getLongValue(byte[], int);
  public static java.math.BigInteger getValue(byte[], int);
  public static long getLongValue(byte[]);
  public static java.math.BigInteger getValue(byte[]);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.feilong.lib.compress.archivers.zip.ZipEncoding`

```java
public interface com.feilong.lib.compress.archivers.zip.ZipEncoding {
  public abstract boolean canEncode(java.lang.String);
  public abstract java.nio.ByteBuffer encode(java.lang.String) throws java.io.IOException;
  public abstract java.lang.String decode(byte[]) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.archivers.zip.ZipEncodingHelper`

```java
public abstract class com.feilong.lib.compress.archivers.zip.ZipEncodingHelper {
  public com.feilong.lib.compress.archivers.zip.ZipEncodingHelper();
  public static com.feilong.lib.compress.archivers.zip.ZipEncoding getZipEncoding(java.lang.String);
}
```

## `com.feilong.lib.compress.archivers.zip.ZipExtraField`

```java
public interface com.feilong.lib.compress.archivers.zip.ZipExtraField {
  public abstract com.feilong.lib.compress.archivers.zip.ZipShort getHeaderId();
  public abstract com.feilong.lib.compress.archivers.zip.ZipShort getLocalFileDataLength();
  public abstract com.feilong.lib.compress.archivers.zip.ZipShort getCentralDirectoryLength();
  public abstract byte[] getLocalFileDataData();
  public abstract byte[] getCentralDirectoryData();
  public abstract void parseFromLocalFileData(byte[], int, int) throws java.util.zip.ZipException;
  public abstract void parseFromCentralDirectoryData(byte[], int, int) throws java.util.zip.ZipException;
}
```

## `com.feilong.lib.compress.archivers.zip.ZipFile`

```java
public class com.feilong.lib.compress.archivers.zip.ZipFile implements java.io.Closeable {
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.io.File) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.lang.String) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.lang.String, java.lang.String) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.io.File, java.lang.String) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.io.File, java.lang.String, boolean) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.io.File, java.lang.String, boolean, boolean) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.nio.channels.SeekableByteChannel) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.nio.channels.SeekableByteChannel, java.lang.String) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.nio.channels.SeekableByteChannel, java.lang.String, java.lang.String, boolean) throws java.io.IOException;
  public com.feilong.lib.compress.archivers.zip.ZipFile(java.nio.channels.SeekableByteChannel, java.lang.String, java.lang.String, boolean, boolean) throws java.io.IOException;
  public java.lang.String getEncoding();
  public void close() throws java.io.IOException;
  public static void closeQuietly(com.feilong.lib.compress.archivers.zip.ZipFile);
  public java.util.Enumeration<com.feilong.lib.compress.archivers.zip.ZipArchiveEntry> getEntries();
  public java.util.Enumeration<com.feilong.lib.compress.archivers.zip.ZipArchiveEntry> getEntriesInPhysicalOrder();
  public com.feilong.lib.compress.archivers.zip.ZipArchiveEntry getEntry(java.lang.String);
  public java.lang.Iterable<com.feilong.lib.compress.archivers.zip.ZipArchiveEntry> getEntries(java.lang.String);
  public java.lang.Iterable<com.feilong.lib.compress.archivers.zip.ZipArchiveEntry> getEntriesInPhysicalOrder(java.lang.String);
  public boolean canReadEntryData(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry);
  public java.io.InputStream getRawInputStream(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry);
  public void copyRawEntries(com.feilong.lib.compress.archivers.zip.ZipArchiveOutputStream, com.feilong.lib.compress.archivers.zip.ZipArchiveEntryPredicate) throws java.io.IOException;
  public java.io.InputStream getInputStream(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry) throws java.io.IOException;
  public java.lang.String getUnixSymlink(com.feilong.lib.compress.archivers.zip.ZipArchiveEntry) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.archivers.zip.ZipLong`

```java
public final class com.feilong.lib.compress.archivers.zip.ZipLong implements java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.compress.archivers.zip.ZipLong(long);
  public com.feilong.lib.compress.archivers.zip.ZipLong(int);
  public com.feilong.lib.compress.archivers.zip.ZipLong(byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipLong(byte[], int);
  public byte[] getBytes();
  public long getValue();
  public int getIntValue();
  public static byte[] getBytes(long);
  public static void putLong(long, byte[], int);
  public void putLong(byte[], int);
  public static long getValue(byte[], int);
  public static long getValue(byte[]);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.Object clone();
  public java.lang.String toString();
}
```

## `com.feilong.lib.compress.archivers.zip.ZipMethod`

```java
public final class com.feilong.lib.compress.archivers.zip.ZipMethod extends java.lang.Enum<com.feilong.lib.compress.archivers.zip.ZipMethod> {
  public static com.feilong.lib.compress.archivers.zip.ZipMethod[] values();
  public static com.feilong.lib.compress.archivers.zip.ZipMethod valueOf(java.lang.String);
  public int getCode();
  public static com.feilong.lib.compress.archivers.zip.ZipMethod getMethodByCode(int);
}
```

## `com.feilong.lib.compress.archivers.zip.ZipShort`

```java
public final class com.feilong.lib.compress.archivers.zip.ZipShort implements java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.compress.archivers.zip.ZipShort(int);
  public com.feilong.lib.compress.archivers.zip.ZipShort(byte[]);
  public com.feilong.lib.compress.archivers.zip.ZipShort(byte[], int);
  public byte[] getBytes();
  public int getValue();
  public static byte[] getBytes(int);
  public static void putShort(int, byte[], int);
  public static int getValue(byte[], int);
  public static int getValue(byte[]);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.Object clone();
  public java.lang.String toString();
}
```

## `com.feilong.lib.compress.archivers.zip.ZipSplitReadOnlySeekableByteChannel`

```java
public class com.feilong.lib.compress.archivers.zip.ZipSplitReadOnlySeekableByteChannel extends com.feilong.lib.compress.utils.MultiReadOnlySeekableByteChannel {
  public com.feilong.lib.compress.archivers.zip.ZipSplitReadOnlySeekableByteChannel(java.util.List<java.nio.channels.SeekableByteChannel>) throws java.io.IOException;
  public static java.nio.channels.SeekableByteChannel forOrderedSeekableByteChannels(java.nio.channels.SeekableByteChannel...) throws java.io.IOException;
  public static java.nio.channels.SeekableByteChannel forOrderedSeekableByteChannels(java.nio.channels.SeekableByteChannel, java.lang.Iterable<java.nio.channels.SeekableByteChannel>) throws java.io.IOException;
  public static java.nio.channels.SeekableByteChannel buildFromLastSplitSegment(java.io.File) throws java.io.IOException;
  public static java.nio.channels.SeekableByteChannel forFiles(java.io.File...) throws java.io.IOException;
  public static java.nio.channels.SeekableByteChannel forFiles(java.io.File, java.lang.Iterable<java.io.File>) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.archivers.zip.ZipUtil`

```java
public abstract class com.feilong.lib.compress.archivers.zip.ZipUtil {
  public com.feilong.lib.compress.archivers.zip.ZipUtil();
  public static com.feilong.lib.compress.archivers.zip.ZipLong toDosTime(java.util.Date);
  public static byte[] toDosTime(long);
  public static void toDosTime(long, byte[], int);
  public static long adjustToLong(int);
  public static byte[] reverse(byte[]);
  public static int signedByteToUnsignedInt(byte);
  public static byte unsignedIntToSignedByte(int);
  public static java.util.Date fromDosTime(com.feilong.lib.compress.archivers.zip.ZipLong);
  public static long dosToJavaTime(long);
}
```
