
Nothing to read...

a lot to read:

asfhisahofhsdofhooooooooooooooooofsjdfpjsdpfjspdjfjsdfjsdfhshdfoshdfohsodfhsohdfohsofhs

#pragma once
#include "betmanager.h"
#include "mainmenu.h"

namespace SaltyBet_Manual {

	using namespace System;
	using namespace System::ComponentModel;
	using namespace System::Collections;
	using namespace System::Windows::Forms;
	using namespace System::Data;
	using namespace System::Drawing;

	/// <summary>
	/// Summary for playernames
	/// </summary>
	public ref class playernames : public System::Windows::Forms::Form
	{

	public:

		int^ nr; //number of player that will come from main menu
		int^ pool; //player bet pool

	public:
		playernames(void)
		{
			InitializeComponent();
			//
			//TODO: Add the constructor code here
			//
		}

		playernames(int^ numberofplayers, int^ playerpool) //overloading the constructor that information is passed
		{
			InitializeComponent();
			nr = numberofplayers;
			pool = playerpool;

			//
			//TODO: Add the constructor code here
			//
		}

	protected:
		/// <summary>
		/// Clean up any resources being used.
		/// </summary>
		~playernames()
		{
			if (components)
			{
				delete components;
			}
		}
	private: System::Windows::Forms::PictureBox^  pictureBox1;
	protected:
	private: System::Windows::Forms::Label^  label1;
	private: System::Windows::Forms::Label^  label2;
	private: System::Windows::Forms::Label^  label3;
	private: System::Windows::Forms::Label^  label4;
	private: System::Windows::Forms::TextBox^  textBox1;
	private: System::Windows::Forms::TextBox^  textBox2;
	private: System::Windows::Forms::TextBox^  textBox3;
	private: System::Windows::Forms::TextBox^  textBox4;
	private: System::Windows::Forms::Label^  label5;
	private: System::Windows::Forms::Button^  button1;
	private: System::Windows::Forms::Button^  button2;
	private: System::Windows::Forms::LinkLabel^  linkLabel1;
	private: System::Windows::Forms::Label^  label6;

	private:
		/// <summary>
		/// Required designer variable.
		/// </summary>
		System::ComponentModel::Container ^components;

#pragma region Windows Form Designer generated code
		/// <summary>
		/// Required method for Designer support - do not modify
		/// the contents of this method with the code editor.
		/// </summary>
		void InitializeComponent(void)
		{
			System::ComponentModel::ComponentResourceManager^  resources = (gcnew System::ComponentModel::ComponentResourceManager(playernames::typeid));
			this->pictureBox1 = (gcnew System::Windows::Forms::PictureBox());
			this->label1 = (gcnew System::Windows::Forms::Label());
			this->label2 = (gcnew System::Windows::Forms::Label());
			this->label3 = (gcnew System::Windows::Forms::Label());
			this->label4 = (gcnew System::Windows::Forms::Label());
			this->textBox1 = (gcnew System::Windows::Forms::TextBox());
			this->textBox2 = (gcnew System::Windows::Forms::TextBox());
			this->textBox3 = (gcnew System::Windows::Forms::TextBox());
			this->textBox4 = (gcnew System::Windows::Forms::TextBox());
			this->label5 = (gcnew System::Windows::Forms::Label());
			this->button1 = (gcnew System::Windows::Forms::Button());
			this->button2 = (gcnew System::Windows::Forms::Button());
			this->linkLabel1 = (gcnew System::Windows::Forms::LinkLabel());
			this->label6 = (gcnew System::Windows::Forms::Label());
			(cli::safe_cast<System::ComponentModel::ISupportInitialize^>(this->pictureBox1))->BeginInit();
			this->SuspendLayout();
			// 
			// pictureBox1
			// 
			this->pictureBox1->Image = (cli::safe_cast<System::Drawing::Image^>(resources->GetObject(L"pictureBox1.Image")));
			this->pictureBox1->Location = System::Drawing::Point(379, 6);
			this->pictureBox1->Name = L"pictureBox1";
			this->pictureBox1->Size = System::Drawing::Size(410, 322);
			this->pictureBox1->SizeMode = System::Windows::Forms::PictureBoxSizeMode::StretchImage;
			this->pictureBox1->TabIndex = 0;
			this->pictureBox1->TabStop = false;
			// 
			// label1
			// 
			this->label1->AutoSize = true;
			this->label1->Location = System::Drawing::Point(12, 76);
			this->label1->Name = L"label1";
			this->label1->Size = System::Drawing::Size(60, 16);
			this->label1->TabIndex = 1;
			this->label1->Text = L"Player 1:";
			// 
			// label2
			// 
			this->label2->AutoSize = true;
			this->label2->Location = System::Drawing::Point(12, 118);
			this->label2->Name = L"label2";
			this->label2->Size = System::Drawing::Size(60, 16);
			this->label2->TabIndex = 2;
			this->label2->Text = L"Player 2:";
			// 
			// label3
			// 
			this->label3->AutoSize = true;
			this->label3->Location = System::Drawing::Point(12, 160);
			this->label3->Name = L"label3";
			this->label3->Size = System::Drawing::Size(60, 16);
			this->label3->TabIndex = 3;
			this->label3->Text = L"Player 3:";
			// 
			// label4
			// 
			this->label4->AutoSize = true;
			this->label4->Location = System::Drawing::Point(12, 199);
			this->label4->Name = L"label4";
			this->label4->Size = System::Drawing::Size(60, 16);
			this->label4->TabIndex = 4;
			this->label4->Text = L"Player 4:";
			// 
			// textBox1
			// 
			this->textBox1->Location = System::Drawing::Point(108, 73);
			this->textBox1->Name = L"textBox1";
			this->textBox1->Size = System::Drawing::Size(177, 22);
			this->textBox1->TabIndex = 5;
			// 
			// textBox2
			// 
			this->textBox2->Location = System::Drawing::Point(108, 112);
			this->textBox2->Name = L"textBox2";
			this->textBox2->Size = System::Drawing::Size(177, 22);
			this->textBox2->TabIndex = 6;
			// 
			// textBox3
			// 
			this->textBox3->Location = System::Drawing::Point(108, 154);
			this->textBox3->Name = L"textBox3";
			this->textBox3->Size = System::Drawing::Size(177, 22);
			this->textBox3->TabIndex = 7;
			// 
			// textBox4
			// 
			this->textBox4->Location = System::Drawing::Point(108, 193);
			this->textBox4->Name = L"textBox4";
			this->textBox4->Size = System::Drawing::Size(177, 22);
			this->textBox4->TabIndex = 8;
			// 
			// label5
			// 
			this->label5->AutoSize = true;
			this->label5->Font = (gcnew System::Drawing::Font(L"Microsoft Sans Serif", 7.488F, System::Drawing::FontStyle::Bold, System::Drawing::GraphicsUnit::Point,
				static_cast<System::Byte>(0)));
			this->label5->Location = System::Drawing::Point(52, 9);
			this->label5->Name = L"label5";
			this->label5->Size = System::Drawing::Size(258, 16);
			this->label5->TabIndex = 9;
			this->label5->Text = L"Please Insert the Player(s) Name(s):";
			// 
			// button1
			// 
			this->button1->Location = System::Drawing::Point(235, 268);
			this->button1->Name = L"button1";
			this->button1->Size = System::Drawing::Size(75, 23);
			this->button1->TabIndex = 10;
			this->button1->Text = L"OK";
			this->button1->UseVisualStyleBackColor = true;
			this->button1->Click += gcnew System::EventHandler(this, &playernames::button1_Click);
			// 
			// button2
			// 
			this->button2->Location = System::Drawing::Point(55, 268);
			this->button2->Name = L"button2";
			this->button2->Size = System::Drawing::Size(75, 23);
			this->button2->TabIndex = 11;
			this->button2->Text = L"Back";
			this->button2->UseVisualStyleBackColor = true;
			this->button2->Click += gcnew System::EventHandler(this, &playernames::button2_Click);
			// 
			// linkLabel1
			// 
			this->linkLabel1->AutoSize = true;
			this->linkLabel1->Location = System::Drawing::Point(192, 315);
			this->linkLabel1->Name = L"linkLabel1";
			this->linkLabel1->Size = System::Drawing::Size(114, 16);
			this->linkLabel1->TabIndex = 13;
			this->linkLabel1->TabStop = true;
			this->linkLabel1->Text = L"www.saltybet.com";
			// 
			// label6
			// 
			this->label6->AutoSize = true;
			this->label6->Location = System::Drawing::Point(83, 315);
			this->label6->Name = L"label6";
			this->label6->Size = System::Drawing::Size(103, 16);
			this->label6->TabIndex = 12;
			this->label6->Text = L"Visit SaltyBet at:";
			// 
			// playernames
			// 
			this->AutoScaleDimensions = System::Drawing::SizeF(8, 16);
			this->AutoScaleMode = System::Windows::Forms::AutoScaleMode::Font;
			this->ClientSize = System::Drawing::Size(801, 340);
			this->Controls->Add(this->linkLabel1);
			this->Controls->Add(this->label6);
			this->Controls->Add(this->button2);
			this->Controls->Add(this->button1);
			this->Controls->Add(this->label5);
			this->Controls->Add(this->textBox4);
			this->Controls->Add(this->textBox3);
			this->Controls->Add(this->textBox2);
			this->Controls->Add(this->textBox1);
			this->Controls->Add(this->label4);
			this->Controls->Add(this->label3);
			this->Controls->Add(this->label2);
			this->Controls->Add(this->label1);
			this->Controls->Add(this->pictureBox1);
			this->Icon = (cli::safe_cast<System::Drawing::Icon^>(resources->GetObject(L"$this.Icon")));
			this->Name = L"playernames";
			this->Text = L"Player Names";
			this->Load += gcnew System::EventHandler(this, &playernames::playernames_Load);
			(cli::safe_cast<System::ComponentModel::ISupportInitialize^>(this->pictureBox1))->EndInit();
			this->ResumeLayout(false);
			this->PerformLayout();

		}
#pragma endregion
	private: System::Void playernames_Load(System::Object^  sender, System::EventArgs^  e) {

		//put code in here for when the systems loads

		switch (System::Convert::ToInt32(nr)) //in order to show only the labels and text boxes tahat are necessary
		{
		case 1:
			// making unnecessary labels invisable
			label2->Visible = false;
			label3->Visible = false;
			label4->Visible = false;

			// making unnecessary text boxes invisable
			textBox2->Visible = false;
			textBox3->Visible = false;
			textBox4->Visible = false;

			break;

		case 2:

			// making unnecessary labels invisable
			label3->Visible = false;
			label4->Visible = false;

			// making unnecessary text boxes invisable
			textBox3->Visible = false;
			textBox4->Visible = false;

			break;

		case 3:

			// making unnecessary labels invisable
			label4->Visible = false;

			// making unnecessary text boxes invisable
			textBox4->Visible = false;

			break;

		default:
			break;
		}


	}
private: System::Void button2_Click(System::Object^  sender, System::EventArgs^  e) {

	//go back to main menu
	this->Hide(); // will close the player names window
	mainmenu^ mm = gcnew mainmenu(); // call the main menu constructor
	mm->ShowDialog(); // will open the main menu

}
private: System::Void button1_Click(System::Object^  sender, System::EventArgs^  e) {

	//go to bet manager menu

	int numberp = System::Convert::ToInt16(nr);
	int np1 = System::Convert::ToInt16(textBox1->Text);
	int np2 = System::Convert::ToInt16(textBox2->Text);
	int np3 = System::Convert::ToInt16(textBox3->Text);
	int np4 = System::Convert::ToInt16(textBox4->Text);


	//go to bet manager
	this->Hide(); // will close the player names window
	betmanager^ bm = gcnew betmanager(numberp, np1, np2, np3, np4); // call the bet manager constructor
	bm->ShowDialog(); // will open the bet manager

}
};
}
