import os
import glob

def cleanup_temp_files(directory):
    # target files with ".tmp" and ".temp" extensions as temporary files
    temp_file_extensions = [".tmp", ".temp"]

    # Get a list of all files with the specified extensions in the directory
    temp_files = []
    for extension in temp_file_extensions:
        temp_files.extend(glob.glob(os.path.join(directory, f"*{extension}")))

    # Delete each temporary file
    for temp_file in temp_files:
        try:
            os.remove(temp_file)
            print(f"Deleted temporary file: {temp_file}")
        except OSError as e:
            print(f"Failed to delete {temp_file}: {e}")

if __name__ == "__main__":
    target_directory = "C:\users\user\temp"  # Change this to the directory you want to clean up
    cleanup_temp_files(target_directory)
